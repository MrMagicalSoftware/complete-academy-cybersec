# Sql Injection


L'SQL injection è una tecnica di attacco informatico che sfrutta le vulnerabilità nelle applicazioni web che interagiscono con un database. Questo tipo di attacco consente a un malintenzionato di inserire o "iniettare" codice SQL malevolo in una query SQL, con l'obiettivo di manipolare il database in modi non autorizzati.

Vulnerabilità: L'SQL injection si verifica quando un'applicazione web non valida correttamente i dati forniti dall'utente. Ad esempio, se un'applicazione accetta input da un modulo di login senza filtrare o sanificare i dati, un attaccante può inserire codice SQL.



Esempio di attacco: Supponiamo che un'applicazione utilizzi una query SQL simile a questa per autenticare un utente:


```
SELECT * FROM utenti WHERE username = 'input_utente' AND password = 'input_password';
```

Se un attaccante inserisce come nome utente admin' --, la query diventa:

```
SELECT * FROM utenti WHERE username = 'admin' --' AND password = 'input_password';
```
In questo caso, il -- commenta il resto della query, quindi l'attaccante riesce ad accedere come utente "admin" senza conoscere la password.

Conseguenze: Gli attacchi di SQL injection possono portare a vari problemi, tra cui:<br>
Accesso non autorizzato ai dati sensibili.<br>
Modifica o cancellazione di dati nel database.<br>
Esecuzione di comandi di sistema sul server.<br>
Esfiltrazione di dati riservati.<br>

Prevenzione: Per proteggere le applicazioni da attacchi di SQL injection, è importante:
Utilizzare query parametrizzate o prepared statements, che separano i dati dal codice SQL.
Validare e sanificare sempre l'input dell'utente.
Implementare controlli di accesso adeguati e monitorare le attività sospette.


________________________________


## In band Sql Injection


L'In-Band SQL Injection è una delle forme più comuni di attacco SQL injection, in cui l'attaccante riesce a ottenere informazioni dal database attraverso il canale di comunicazione già utilizzato per inviare le richieste. In altre parole, l'attaccante sfrutta la stessa connessione per inviare comandi SQL malevoli e ricevere i risultati.


Ci sono due sottotipi principali di In-Band SQL Injection:

1. **Error-Based SQL Injection**: In questo caso, l'attaccante provoca un errore nel database che rivela informazioni utili. Ad esempio, se l'attaccante inserisce un input progettato per generare un errore, il messaggio di errore restituito dal database può contenere dettagli sulla struttura del database, come nomi di tabelle o colonne. Questo tipo di attacco è utile per raccogliere informazioni sul database.

   **Esempio**: Se l'attaccante inserisce un input come `1' AND 1=CONVERT(int, (SELECT @@version)) --`, il database potrebbe restituire un errore che rivela la versione del database in uso.

2. **Union-Based SQL Injection**: Questo tipo di attacco sfrutta l'operatore `UNION` per combinare i risultati di più query. L'attaccante può utilizzare questa tecnica per estrarre dati da altre tabelle nel database. Per farlo, l'attaccante deve conoscere il numero di colonne nella query originale e il tipo di dati che ciascuna colonna restituisce.

   **Esempio**: Se l'applicazione originale esegue una query come `SELECT nome, email FROM utenti WHERE id = 1`, l'attaccante potrebbe iniettare un input come `1 UNION SELECT username, password FROM admin --`. Questo restituirebbe i nomi utente e le password dalla tabella "admin".

### Prevenzione dell'In-Band SQL Injection

Per proteggere le applicazioni da attacchi di In-Band SQL Injection, è fondamentale adottare le seguenti misure:

- **Utilizzare Prepared Statements**: Le query parametrizzate separano i dati dal codice SQL, riducendo il rischio di iniezione.
- **Sanificare l'Input**: Validare e filtrare sempre i dati forniti dagli utenti per rimuovere caratteri pericolosi.
- **Limitare i Messaggi di Errore**: Non rivelare informazioni dettagliate sugli errori del database agli utenti finali, poiché possono fornire indizi utili agli attaccanti.
- **Implementare Controlli di Accesso**: Assicurarsi che solo gli utenti autorizzati possano accedere a determinate informazioni o funzionalità.


## Pratical 


The key to discovering error-based SQL Injection is to break the code's SQL query by trying certain characters until an error message is produced; these are most commonly single apostrophes ( ' ) or a quotation mark ( " ).


Try typing an apostrophe ( ' ) after the id=1 and press enter. And you'll see this returns an SQL error informing you of an error in your syntax. The fact that you've received this error message confirms the existence of an SQL Injection vulnerability. We can now exploit this vulnerability and use the error messages to learn more about the database structure.



https://website.thm/article?id=1 UNION SELECT 1

La parte UNION SELECT 1 è ciò che rende questa query un tentativo di SQL injection.

UNION: L'operatore UNION combina i risultati di due o più query SELECT. Per funzionare correttamente, le query devono avere lo stesso numero di colonne e tipi di dati compatibili.
SELECT 1: Questa parte della query seleziona semplicemente il valore 1. Non specifica alcuna tabella, quindi non sta cercando di estrarre dati da una tabella esistente.










