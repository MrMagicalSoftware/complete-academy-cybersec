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




