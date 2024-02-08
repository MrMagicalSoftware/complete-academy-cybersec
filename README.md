# complete-academy-cybersec

# Definizione di Networking

Il networking, in termini informatici e tecnologici, si riferisce alla pratica di collegare tra loro dispositivi hardware (come computer, stampanti, server, switch, router e altri dispositivi) e software al fine di scambiare dati e condividere risorse all’interno di un sistema come una rete aziendale o su Internet stessa. Questa connessione può avvenire tramite cavi (rete cablata) o wireless (rete senza fili).

Il networking abbraccia una varietà di concetti tecnologici, tra cui:

1. Reti LAN e WAN: Local Area Network (LAN) si riferisce a una rete in un’area limitata, come un ufficio o una casa, mentre Wide Area Network (WAN) copre aree geograficamente più ampie, potenzialmente su scala globale, come Internet.

2. Protocolli di rete: I protocolli di rete sono insiemi di regole che governano la comunicazione tra dispositivi in rete. Esempi comuni sono l’Internet Protocol (IP), il Transmission Control Protocol (TCP), e il Hypertext Transfer Protocol (HTTP).

3. Hardware di rete: Includono dispositivi come router, switch, hub, modems, access points, e le infrastrutture di trasmissione che permettono il passaggio del traffico di rete tra dispositivi.

4. Topologia di rete: Si riferisce alla disposizione fisica o logica di una rete, inclusi i percorsi utilizzati per scambiare dati tra nodi di rete, come una topologia a stella, ad anello, a maglia o ad albero.

5. Architetture di rete: Il modo in cui i componenti di una rete sono organizzati e interagiscono, come client-server o peer-to-peer (P2P).

6. Cybersecurity: Il networking comporta anche la sicurezza della rete, che consiste nel proteggere le risorse di rete e i dati trasferiti da minacce come attacchi informatici, malware e intrusioni.

Il networking è fondamentale per il funzionamento delle moderne società informatiche, facilitando applicazioni come email, condivisione di file, accesso a risorse remote, streaming di media, comunicazioni VoIP e la connettività Internet in generale. Inoltre, con l’avvento di tecnologie come l’Internet of Things (IoT), il networking ha esteso la sua portata connettendo anche dispositivi non tradizionali, come elettrodomestici, veicoli e sensori, contribuendo a costruire ambienti intelligenti e interconnessi.

# IP ADDRESSES

Il Protocollo Internet, comunemente noto con la sigla IP (dall’inglese “Internet Protocol”), è uno dei principali protocolli di rete su cui si fonda Internet. Si occupa di indirizzare e instradare i pacchetti di dati tra host su reti interconnesse, permettendo così ai dispositivi di comunicare tra di loro indipendentemente dalla loro posizione fisica o dalla topologia di rete impiegata.

### Funzionamento Base del Protocollo IP:

Indirizzamento IP:
Ogni dispositivo collegato a una rete TCP/IP ha assegnato un indirizzo IP univoco, che essenzialmente funge da identificativo del dispositivo sulla rete. L’indirizzo IP è composto da una serie di numeri divisi in segmenti, standardmente rappresentati in forma decimale per IPv4 (ad esempio, 192.168.1.1) o in forma esadecimale per IPv6 (ad esempio, 2001:0db8:85a3:0000:0000:8a2e:0370:7334).

Instradamento:
Gli indirizzi IP sono utilizzati dai router, che sono dispositivi specializzati per instradare il traffico di rete, per determinare il percorso migliore attraverso il quale un pacchetto di dati può viaggiare dalla sorgente alla destinazione. L’inoltro dei pacchetti si basa su tabelle di routing che tengono traccia delle reti adiacenti e dei percorsi ottimali per raggiungere specifiche sottoreti.

Pacchettizzazione:
IP è un protocollo senza connessione, il che significa che i dati inviati sono suddivisi in pacchetti che viaggiano in modo indipendente attraverso la rete. Ogni pacchetto contiene l’indirizzo IP di origine e di destinazione oltre a una sequenza di dati. Poiché i pacchetti possono percorrere percorsi diversi per raggiungere la destinazione, possono arrivare in ordine diverso da quello di partenza, oppure alcuni potrebbero non arrivare affatto.

### Versioni di IP:

Esistono due versioni principali del Protocollo Internet in uso:

IPv4 (IP version 4):
Questa è la versione più diffusa di IP, ed è stata la spina dorsale di Internet fin dalla sua invenzione. Gli indirizzi IPv4 sono lunghi 32 bit, per un totale di circa 4,3 miliardi di indirizzi unici possibili. Tuttavia, a causa dell’enorme crescita di dispositivi collegati a Internet, gli indirizzi IPv4 stanno andando esauriti.

IPv6 (IP version 6):
IPv6 è stato introdotto per risolvere il problema dell’esaurimento degli indirizzi IPv4. Gli indirizzi IPv6 sono lunghi 128 bit, offrendo un numero quasi infinito di indirizzi IP disponibili (2^128, ossia circa 340 undecillioni di indirizzi). IPv6 offre anche miglioramenti in termini di efficienza del routing, sicurezza e facilità di configurazione dei dispositivi di rete.

### Importanza del Protocollo IP:

Il Protocollo IP è essenziale per il funzionamento di Internet e delle reti moderne. Oltre a permettere la comunicazione tra dispositivi distantissimi, agevola l’autoconfigurazione e il dynamic host configuration, elementi basilari per la gestione e la scalabilità di grandi reti. Inoltre, la transizione verso IPv6 gioca un ruolo cruciale per sostenere lo sviluppo futuro dell’Internet of Things (IoT) e per supportare un numero sempre crescente di dispositivi connessi.

______________________________________


# Esempio di IP address :

172.16.254.1 , l'ip è composto da 32 bit ( 4 bytes ).
Ricordando che 1 bytes -> 8 bit 


<img width="365" alt="Screenshot 2024-02-08 alle 10 57 44" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/4fa494a3-0a37-4bf9-9a5e-2d81a9e7ab86">



<img width="405" alt="Screenshot 2024-02-08 alle 11 00 21" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/5b2257b0-efe6-4170-b15a-2a0e81a64f32">




# Panoramica sulle classi di ip



Le classi di indirizzi IP definiscono gruppi di indirizzi IPv4 che sono divisi in blocchi basati sulla loro destinazione originale e capacità della rete. L’impostazione delle classi di indirizzo IP era le fondamenta del sistema originale di indirizzamento IP, che è stato successivamente affinato con l’introduzione della notazione CIDR (Classless Inter-Domain Routing) per un uso più efficiente dello spazio di indirizzamento.

Class A: 0.0.0.0 - 127.255.255.255
Class B: 128.0.0.0 - 191.255.255.255
Class C: 192.0.0.0 - 223.255.255.255

Ogni classe di indirizzi IP aveva una finalità specifica, ma questo schema si è rivelato inefficiente con il passare del tempo e l’espansione di Internet. L’introduzione della CIDR ha permesso di allocare gli indirizzi IP in modo più flessibile, basato su esigenze di rete variabili piuttosto che su un sistema di classi fisse, mitigando la rapida esauribilità dell’IPv4.

Gli indirizzi IP attuali vengono quindi distribuiti e gestiti in maniera “classless”, con blocchi di indirizzi allocati a enti e organizzazioni in base ai loro specifici bisogni e con netmask (o prefissi) di varie lunghezze, consentendo un uso più granulare e ottimizzato dell’indirizzamento IP.


# PUBLIC VS PRIVATE IP ADDRESSES


È importante notare che il nostro sistema di indirizzi IP ha dei limiti.
Il limite più significativo è che non ci sono abbastanza indirizzi IP per coprire tutti i dispositivi che devono connettersi a Internet. 
Il sistema IPv4 con cui lavoriamo oggi ha solo 4,3 miliardi di indirizzi IP. Con 7,5 miliardi di persone sul pianeta e un numero molto più elevato di dispositivi, questo non è certamente sufficiente.
Di conseguenza, è stato sviluppato un sistema per riutilizzare un gruppo di indirizzi IP all'interno di una LAN, che non sono utilizzabili su Internet. 
Questi indirizzi possono essere utilizzati più volte all'interno di ogni rete locale, ma non su Internet, conservando così il numero di indirizzi IP

Questi indirizzi privati includono:

192.168.0.0 - 192.168.255.255
10.0.0.0 - 10.255.255.255
172.16.0.0 - 172.16.255.255


<img width="200" alt="Screenshot 2024-02-08 alle 11 15 30" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/6ccec07b-fc1f-4347-81f7-60d8f40a86d6">


This is your private IP that is only usable on the local area network.
To communicate over the internet, your IP address must be translated to a public IP by a NAT device


> ifconfig


# APPROFONDIMENTO IFCONFIG


comandi `ifconfig`:

1. **Visualizzare tutte le interfacce di rete disponibili:**
   ```bash
   ifconfig -a
   ```

2. **Visualizzare informazioni dettagliate per una specifica interfaccia di rete (ad esempio, eth0):**
   ```bash
   ifconfig eth0
   ```

3. **Attivare un'interfaccia di rete (ad esempio, eth0):**
   ```bash
   sudo ifconfig eth0 up
   ```

4. **Disattivare un'interfaccia di rete (ad esempio, eth0):**
   ```bash
   sudo ifconfig eth0 down
   ```

5. **Assegnare un indirizzo IP statico a un'interfaccia di rete (ad esempio, eth0):**
   ```bash
   sudo ifconfig eth0 192.168.1.2 netmask 255.255.255.0
   ```

6. **Impostare un indirizzo IP e una metrica manualmente:**
   ```bash
   sudo ifconfig eth0 192.168.1.2 metric 1
   ```

7. **Cambiare il MAC address di un'interfaccia (ad esempio, eth0):**
   ```bash
   sudo ifconfig eth0 hw ether 00:11:22:33:44:55
   ```

8. **Abilitare la modalità promiscua su un'interfaccia di rete (ad esempio, eth0):**
   ```bash
   sudo ifconfig eth0 promisc
   ```

9. **Disabilitare la modalità promiscua su un'interfaccia di rete (ad esempio, eth0):**
   ```bash
   sudo ifconfig eth0 -promisc
   ```

10. **Visualizzare solo le informazioni sull'indirizzo IP di tutte le interfacce di rete:**
    ```bash
    ifconfig | grep "inet addr"
    ```


# COMANDO WINDOWS :

> ipconfig


Il comando `ipconfig` è utilizzato su sistemi operativi Windows per visualizzare e gestire le configurazioni di rete.

1. **Visualizzare tutte le informazioni sulla configurazione di rete:**
   ```bash
   ipconfig
   ```

2. **Visualizzare informazioni dettagliate su tutte le interfacce di rete:**
   ```bash
   ipconfig /all
   ```

3. **Rinnovare l'assegnazione dell'indirizzo IP da un server DHCP:**
   ```bash
   ipconfig /renew
   ```

4. **Rilasciare l'indirizzo IP assegnato da un server DHCP:**
   ```bash
   ipconfig /release
   ```

5. **Visualizzare solo l'indirizzo IP per tutte le interfacce di rete:**
   ```bash
   ipconfig | findstr "IPv4"
   ```

6. **Visualizzare le informazioni sulla configurazione DNS:**
   ```bash
   ipconfig /all | findstr "DNS"
   ```

7. **Visualizzare solo l'indirizzo IP di un'interfaccia specifica (ad esempio, Ethernet):**
   ```bash
   ipconfig | findstr "Ethernet" -A 3
   ```

8. **Visualizzare l'indirizzo IP e il gateway predefinito di un'interfaccia specifica (ad esempio, Wi-Fi):**
   ```bash
   ipconfig | findstr "Wi-Fi" -A 5
   ```

9. **Visualizzare solo l'indirizzo MAC di tutte le interfacce di rete:**
   ```bash
   ipconfig /all | findstr "Physical Address"
   ```

10. **Visualizzare solo le informazioni sulla subnet mask di tutte le interfacce di rete:**
    ```bash
    ipconfig | findstr "Subnet Mask"
    ```


___________________________________________________________________________________________


# COMANDO IP (SISTEMI LINUX )

Comando preferibile rispetto ad ifconfig


Il comando `ip` su Linux è un potente strumento di configurazione di rete che offre molte funzionalità avanzate rispetto al più tradizionale `ifconfig`.

1. **Visualizzare tutte le informazioni sulle interfacce di rete:**
   ```bash
   ip addr show
   ```

2. **Visualizzare informazioni specifiche su un'interfaccia di rete (ad esempio, eth0):**
   ```bash
   ip addr show eth0
   ```

3. **Attivare un'interfaccia di rete (ad esempio, eth0):**
   ```bash
   sudo ip link set dev eth0 up
   ```

4. **Disattivare un'interfaccia di rete (ad esempio, eth0):**
   ```bash
   sudo ip link set dev eth0 down
   ```

5. **Assegnare un indirizzo IP statico a un'interfaccia di rete (ad esempio, eth0):**
   ```bash
   sudo ip addr add 192.168.1.2/24 dev eth0
   ```

6. **Rimuovere un indirizzo IP da un'interfaccia di rete (ad esempio, eth0):**
   ```bash
   sudo ip addr del 192.168.1.2/24 dev eth0
   ```

7. **Visualizzare la tabella di routing:**
   ```bash
   ip route show
   ```

8. **Aggiungere una rotta statica:**
   ```bash
   sudo ip route add 192.168.2.0/24 via 192.168.1.1 dev eth0
   ```

9. **Cambiare il MAC address di un'interfaccia (ad esempio, eth0):**
   ```bash
   sudo ip link set dev eth0 address 00:11:22:33:44:55
   ```

10. **Abilitare la modalità promiscua su un'interfaccia di rete (ad esempio, eth0):**
    ```bash
    sudo ip link set dev eth0 promisc on
    ```

11. **Disabilitare la modalità promiscua su un'interfaccia di rete (ad esempio, eth0):**
    ```bash
    sudo ip link set dev eth0 promisc off
    ```


# PROTOCOLLO DHCP

<img width="526" alt="Screenshot 2024-02-08 alle 14 14 21" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/be35623b-cb0e-466c-a0e8-bfbd209dfa6e">




Il protocollo DHCP (Dynamic Host Configuration Protocol) è un protocollo di rete utilizzato per assegnare automaticamente gli indirizzi IP e altri parametri di configurazione di rete ai dispositivi client, consentendo loro di connettersi a una rete senza richiedere intervento manuale. DHCP è ampiamente utilizzato in quasi tutte le reti moderne, incluse quelle domestiche, aziendali e pubbliche.

Funzionamento di DHCP:

Quando un dispositivo (client) si connette a una rete, segue un processo DHCP a quattro fasi, noto anche come DORA (Discover, Offer, Request, Acknowledge):

1. Discover: Il client invia un messaggio broadcast (a tutti i dispositivi nella rete) chiamato DHCP Discover per cercare server DHCP disponibili.

2. Offer: I server DHCP che ricevono il messaggio Discover rispondono con un messaggio DHCP Offer, che include un indirizzo IP che il server è disposto ad assegnare al client, oltre ad altre informazioni di configurazione come il lease time (il tempo per cui l’indirizzo può essere utilizzato), il gateway predefinito, e i server DNS.

3. Request: Il client riceve una o più offerte e sceglie una. Poi invia un messaggio broadcast DHCP Request per informare tutti i server DHCP sulla scelta dell’offerta accettata e per richiedere l’indirizzo IP proposto.

4. Acknowledge: Il server DHCP selezionato risponde con un messaggio DHCP Acknowledge, confermando l’assegnazione dell’indirizzo IP e di altri parametri di configurazione al client. Se invece avviene un problema, il server invierà un messaggio DHCP Nak (negative acknowledgment), e il client dovrà iniziare nuovamente il processo.

Esempio:

Si immagini di  avere un router domestico con DHCP abilitato e un nuovo smartphone che vuoi connettere alla tua rete Wi-Fi.

1. Discover: Il tuo smartphone si connette alla rete Wi-Fi e automaticamente invia un messaggio di Discover per cercare un server DHCP nella rete per ottenere un indirizzo IP.

2. Offer: Il router, agendo come server DHCP, riceve il messaggio di Discover e risponde al tuo smartphone con un’offerta che include un indirizzo IP disponibile, ad esempio 192.168.1.10, insieme al lease time (es. 24 ore), l’indirizzo del gateway (il router stesso, ad esempio 192.168.1.1), e gli indirizzi dei server DNS (es. 8.8.8.8, fornito da Google).

3. Request: Il tuo smartphone seleziona questa offerta e invia un messaggio di Request indietro al router per accettare l’indirizzo IP di 192.168.1.10.

4. Acknowledge: Il router conferma la selezione inviando al tuo smartphone un messaggio Acknowledge e allo stesso tempo aggiorna la sua tabella di allocazione DHCP per indicare che l’indirizzo 192.168.1.10 è ora assegnato al tuo smartphone per la durata del lease.

Dopo l’acknowledge, il tuo smartphone può comunicare con altri dispositivi nella rete locale e su internet utilizzando l’indirizzo IP assegnato.

Il processo è completamente trasparente e si svolge in pochi secondi, il che lo rende uno degli elementi chiave per la semplicità e l’efficienza delle moderne reti di computer.


# PROTOCOLLO NAT


Il protocollo NAT (Network Address Translation) è una tecnica utilizzata in reti di computer per trasformare gli indirizzi IP utilizzati all’interno di una rete privata in indirizzi IP utilizzabili su Internet, e viceversa. Tale processo è vitale per consentire ai dispositivi con indirizzi IP privati (che non sono univoci e non possono essere utilizzati su Internet) di comunicare con dispositivi esterni alla loro rete locale.

Le reti private comunemente usano una gamma di indirizzi IP specificata dalla RFC 1918, che non si sovrappone con gli indirizzi IP assegnati su Internet. Questo risulta necessario per evitare esaurimento degli indirizzi IPv4, dato che questi indirizzi sono limitati in numero. NAT permette a molteplici dispositivi su una rete privata di condividere un singolo indirizzo IP pubblico.

Esempio di NAT:

Immagina di avere una rete domestica con vari dispositivi (PC, smartphone, tablet, ecc.) che utilizzano indirizzi IP assegnati privatamente dal tuo router, ad esempio 192.168.1.2, 192.168.1.3, ecc. Il tuo router è l’unico dispositivo nella tua rete che possiede un indirizzo IP pubblico, ad esempio 203.0.113.5, assegnato dal fornitore di servizi Internet (ISP).

Supponiamo che uno dei tuoi dispositivi, diciamo il PC con l’indirizzo IP 192.168.1.2, voglia connettersi a un sito web Internet. Ecco come funzionerebbe con NAT:

1. Il tuo PC inizia inviando una richiesta di connessione TCP alla destinazione sul web, usando il suo indirizzo IP privato come sorgente e l’indirizzo IP del sito web come destinazione.

2. Il router riceve la richiesta e utilizza NAT per modificare l’indirizzo IP sorgente da 192.168.1.2 (privato) in 203.0.113.5 (pubblico), cambiando anche il numero di porta sorgente in uno univoco che tiene traccia della sessione (per esempio 12345).

3. Il router invia la richiesta modificata a Internet, dove il sito web vede la richiesta come proveniente dall’indirizzo IP pubblico del router (203.0.113.5 con porta 12345), non sapendo nulla del dispositivo reale all’interno della tua rete.

4. Quando il sito web risponde, invia i dati al tuo indirizzo IP pubblico (203.0.113.5 con porta 12345).

5. Il router riceve la risposta e attraverso una tabella di traduzione NAT, determina a quale dispositivo e porta interna inoltrare i dati. In questo caso, riconosce che la porta 12345 corrisponde alla sessione originata dal PC all’indirizzo 192.168.1.2.

6. Il router trasforma nuovamente il pacchetto invertendo la traduzione NAT, sostituendo l’indirizzo IP pubblico e la porta con l’indirizzo IP privato e la porta originale del PC (192.168.1.2), e invia i dati al PC.

Spiegazione:

In sostanza, NAT consente ai dispositivi all’interno di una rete privata di utilizzare un unico indirizzo IP pubblico per tutte le loro comunicazioni esterne. Il router tiene traccia delle sessioni usando le porte di rete al fine di distinguere quale traffico in ingresso dai server web (o da altri servizi Internet) deve essere inoltrato a quale dispositivo all’interno della rete privata.

Questo processo consente di risparmiare indirizzi IP (dato che ce ne sono meno di quanti sarebbero necessari altrimenti) e fornisce un livello di sicurezza aggiunto, nascondendo gli indirizzi IP privati dei dispositivi dall’esterno della rete domestica. Tuttavia, NAT può introdurre complicazioni per alcuni protocolli di rete che richiedono la connettività in entrata o che necessitano di conoscere l’indirizzo IP reale del dispositivo, e per questo possono essere necessarie configurazioni aggiuntive come il port forwarding.


# PORTE

PRINCIPALI PORTE : 
https://it.wikipedia.org/wiki/Porte_TCP_e_UDP_standard



Le porte sono un tipo di sottoindirizzo. L'indirizzo IP è l'indirizzo principale, mentre la porta è il sottoindirizzo. Utilizzando una metafora ben collaudata ma efficace, si pensi all'indirizzo IP come all'indirizzo stradale di un edificio e alla porta come al numero dell'appartamento. L'indirizzo stradale mi serve per arrivare all'edificio corretto, ma l'indirizzo dell'appartamento mi serve per trovare la singola persona. Questo è simile alle porte. L'indirizzo IP ci porta all'host giusto, ma la porta ci porta al servizio appropriato, ad esempio HTTP sulla porta 80.
Esistono 65.536 porte (2 elevato alla sedicesima potenza). Le prime 1.024 sono generalmente chiamate "porte comuni".


Le porte TCP (Transmission Control Protocol) e UDP (User Datagram Protocol) sono assegnazioni numeriche utilizzate nei protocolli di rete per distinguere tra diversi servizi o applicazioni che si eseguono su un singolo dispositivo. Entrambi fanno parte della suite di protocolli internet (TCP/IP) e agiscono come meccanismi di indirizzamento all’interno di una rete, in particolare a livello di trasporto (il quarto livello nel modello OSI o il terzo livello nel modello internet).

TCP è un protocollo orientato alla connessione, garantendo che tutti i pacchetti inviati siano ricevuti correttamente e nell’ordine corretto. Riesce a gestire la riconsegna dei pacchetti persi e gestisce il controllo di flusso e la congestione della rete.

UDP è un protocollo senza connessione, non garantisce l’ordine di arrivo o la consegna dei pacchetti, rendendolo più leggero e più veloce di TCP, ma meno affidabile. È utile per servizi che richiedono trasmissioni veloci e in tempo reale, come lo streaming video, i giochi online e le chiamate VoIP, dove la perdita di qualche pacchetto è accettabile e meno critica.

Come funzionano le porte TCP/UDP:

Quando i dati vengono inviati attraverso la rete, sono divisi in piccoli pezzi detti pacchetti. Ogni pacchetto include un’intestazione (header) con diverse informazioni, tra cui il numero di porta sorgente e il numero di porta di destinazione. Questi numeri di porte indicano quale programma o servizio dovrà gestire quel pacchetto.

Ad esempio, se apri un sito web, il tuo browser utilizza il protocollo HTTP o HTTPS, che di default sono assegnati rispettivamente alle porte TCP 80 e 443. Quando fai una richiesta web, il pacchetto viene inviato alla porta 80 o 443 sul server web di destinazione.

Esempi comuni di porte TCP/UDP:

- HTTP (per i siti web): porta TCP 80
- HTTPS (per i siti web sicuri): porta TCP 443
- FTP (File Transfer Protocol): porte TCP 20 (per il trasferimento dati) e 21 (per il controllo della connessione)
- SMTP (Simple Mail Transfer Protocol, per l’invio di email): porta TCP 25
- IMAP (Internet Message Access Protocol, per ricevere email): porta TCP 143
- DNS (Domain Name System): porta UDP 53 (anche TCP per le risposte di dimensioni maggiori)
- DHCP (Dynamic Host Configuration Protocol): porte UDP 67 e 68
- RTP (Real-time Transport Protocol, spesso utilizzato nelle applicazioni di streaming multimediale): porte UDP nell’intervallo dinamico (solitamente da 16384 a 32767)

Le porte vanno da 0 a 65535. Di queste, le porte da 0 a 1023 sono considerate “porte ben note” e sono riservate per servizi ben definiti e ampiamente usati come quelli sopra elencati. Le porte da 1024 a 49151 sono “porte registrate” assegnate per l’uso da protocolli e applicazioni specifici. Infine, le porte da 49152 a 65535 sono “porte dinamiche” o “private”, spesso utilizzate per comunicazioni peer-to-peer o sessioni temporanee


<b>TOOL nmap </b>
 
 ```bash
   sudo nmap –sT <IP address of the target system>
 ```bash


# NOTA
A protocol simply defines a way of communication with all its rules. These rules are usually defined by an RFC (Request for Comments).
There are many, many protocols in use on the internet. These include TCP, IP, UDP, FTP, HTTP, SMTP, etc., and each has its own set of rules that must be complied with to communicate effectively (similar to the rules we use in communication via written languages).


PROTOCOLLO PRINCIPE TCP/IP





# PROTOCOLLO IP ( INTERNET PROTOCOL ) 













