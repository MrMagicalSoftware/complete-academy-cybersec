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
 
 ```

   sudo nmap –sT <IP address of the target system>

 ```






# NOTA
A protocol simply defines a way of communication with all its rules. These rules are usually defined by an RFC (Request for Comments).
There are many, many protocols in use on the internet. These include TCP, IP, UDP, FTP, HTTP, SMTP, etc., and each has its own set of rules that must be complied with to communicate effectively (similar to the rules we use in communication via written languages).


PROTOCOLLO PRINCIPE TCP/IP





# PROTOCOLLO IP ( INTERNET PROTOCOL ) 


Iniziamo a vedere una panoramica generale su questo protocollo :


Il protocollo IP (Internet Protocol) è un protocollo fondamentale nella suite di protocolli TCP/IP ed è l’elemento principale che regola l’instradamento dei dati attraverso reti interconnesse, ovvero Internet. Agisce a livello di rete nel modello OSI, che è il terzo strato del modello di rete. Le due versioni principali sono IPv4 (Protocollo Internet versione 4) e IPv6 (versione 6).

Il compito principale di IP è la consegna di pacchetti dal mittente al destinatario basandosi sui loro indirizzi IP. Un indirizzo IP è un’etichetta numerica univoca assegnata a ogni dispositivo collegato a una rete informatica che utilizza il protocollo IP per comunicare.

IPv4 utilizza indirizzi a 32 bit, che sono comunemente rappresentati in notazione decimale puntata (ad esempio, 192.0.2.1). Tuttavia, poiché il numero di dispositivi connessi a Internet ha superato il numero di indirizzi IPv4 disponibili, è stato sviluppato IPv6.

IPv6 usa indirizzi a 128 bit, offrendo una fornitura praticamente illimitata di indirizzi univoci e è rappresentato in notazione esadecimale, come in questo esempio: 2001:0db8:85a3:0000:0000:8a2e:0370:7334.

Entrambe le versioni del protocollo IP forniscono funzioni che possono essere suddivise in vari aspetti chiave:

1. Indirizzamento e routing: IP assegna indirizzi logici ai dispositivi e gestisce il routing dei pacchetti di dati tra sorgente e destinazione attraverso reti interconnesse.

2. Frammentazione e riassemblaggio: IP è responsabile della frammentazione e del riassemblaggio dei pacchetti. Se un pacchetto è troppo grande per essere trasmesso su una rete, IP lo divide in frammenti di dimensioni gestibili. Questi frammenti vengono poi riassemblati una volta che raggiungono la destinazione.

3. Inoltro di pacchetti: I router utilizzano le intestazioni IP per prendere decisioni sull’inoltro (forwarding) di pacchetti attraverso la rete.

4. Controllo degli errori: IP utilizza un checksum nell’intestazione del pacchetto per verificare l’integrità dei dati dell’intestazione stessa. Se un pacchetto è danneggiato, viene scartato. (Si noti che il controllo degli errori per il contenuto del pacchetto è gestito da protocolli di livello superiore come TCP o UDP).

5. Incapacità di garantire la consegna affidabile: IP non garantisce la consegna affidabile di pacchetti, non mantiene l’ordine di inoltro e non tiene traccia della consegna. Protocolli come TCP sono costruiti sopra IP per fornire questi servizi.


<b>In sintesi </b>
IP, o Internet Protocol, è il protocollo utilizzato per definire l'indirizzo IP di origine e di destinazione di un pacchetto che attraversa Internet. Viene spesso utilizzato insieme ad altri protocolli, come il TCP; da qui la congiunzione spesso usata, TCP/IP.


<b> Anatomia di IP </b>


<img width="865" alt="Screenshot 2024-02-08 alle 14 52 22" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/bf490c78-8985-4143-9241-81fe15bbf17c">


Spiegazione in dettaglio


Row 1
Version: This defines the version of IP, either v4 or v6.
IHL: Defines the header length.
Type of Service (TOS): This defines the type of service of this packet. These include
minimize delay, maximize throughput, maximize reliability, and minimize monetary cost.
Total Length: This defines the total length of the IP datagram (including the data) or the
fragment. Its maximum value is 65,535.


<b>Spiegazione</b>

IHL “Internet Header Length” (Lunghezza Intestazione Internet) ed è un campo presente nell’intestazione di un pacchetto IP. Si trova all’inizio dell’intestazione di un pacchetto IPv4 e specifica la lunghezza dell’intestazione del pacchetto IP in unità di parole a 32 bit.

A causa della possibilità di includere opzioni varie nell’intestazione IP, la lunghezza dell’intestazione non è fissa e può variare. L’IHL indica quanta parte del pacchetto totale è occupata dall’intestazione, consentendo al ricevitore di determinare dove inizia effettivamente il contenuto dati (o payload) del pacchetto.

Per esempio, la lunghezza minima dell’intestazione di un pacchetto IPv4 è di 20 byte (che corrispondono a 5 parole a 32 bit). Qualora non ci siano opzioni IP aggiuntive, il valore dell’IHL sarebbe quindi 5. Se ci fossero opzioni aggiuntive, l’intestazione sarebbe più lunga e il valore di IHL aumenterebbe di conseguenza. Il valore massimo di IHL è 15, indicando una lunghezza massima dell’intestazione di 60 byte.

In caso il pacchetto IP non contenga opzioni, l’IHL avrà il valore tipico di 5. Qualsiasi valore superiore indica la presenza di opzioni nell’intestazione. Questo campo è essenziale per consentire ai dispositivi di rete, come i router, di processare correttamente i pacchetti IP e gestire il payload corrispondente in modo appropriato.



<b> TOS </b>

Il campo Type of Service (ToS) nel protocollo Internet versione 4 (IPv4) era originariamente inteso per permettere ai dispositivi di rete di fornire un trattamento differenziato ai pacchetti IP in base alle loro esigenze di servizio. Il campo ToS è lungo 8 bit e si trova nell’intestazione di un pacchetto IPv4. L’intenzione era quella di utilizzare questo campo per specificare parametri come la priorità del traffico, la qualità del servizio (QoS) e la richiesta di servizi come una latenza ridotta, un’elevata affidabilità o un basso costo per il trasferimento dei dati.


l’intenzione originale del campo ToS era quella di fornire un modo per le sorgenti di pacchetti di esprimere le loro preferenze per come i pacchetti venissero trattati alla consegna. Con la moderna QoS e DiffServ, le funzionalità del campo ToS sono state ampliate e migliorate per fornire un controllo ancora più granulare e una gestione più efficace del traffico di rete.

Il campo ToS si divideva originally in diversi bit con funzioni diverse:

1. Precedence (3 bit più significativi): Indicava la priorità del pacchetto con valori che andavano da 0 (normale priorità) a 7 (priorità più alta). Con sette livelli di priorità possibili, i pacchetti potevano essere instradati in modo da favorire quelli con un livello di priorità più alto in caso di congestione di rete.

2. Delayed (D bit): Indicava se il pacchetto doveva essere ottimizzato per la latenza ridotta.

3. Throughput (T bit): Stabiliva se l’obiettivo era massimizzare la quantità di dati trasferibili.

4. Reliability (R bit): Specificava se la affidabilità (ad esempio, meno errori e meno perdite di pacchetti) era più importante rispetto alle altre metriche.

5. Cost (C bit): Indicava se il percorso a basso costo era preferito rispetto a quelli a maggiore larghezza di banda o affidabilità.

6. I restanti bit (2 bit) erano in origine non utilizzati o riservati per usi futuri.

_______________________


<b> Riga 2 </b>

Identification: This field uniquely identifies each packet. It can be critical in reassembling fragmented packets.<br><br>

IP Flags: This field defines whether the packet is fragmented (M) or not (D). 
The manipulation of the field can be used to evade IDS and firewalls. 
It can also be used in conjunction with the Window field to identify the operating system of the sender.

Fragment Offset: This field is used when packets are fragmented. It defines where the
packets should be reassembled from the beginning of the IP header.


_____________________


<b> Riga 3 </b>

Row 3
TTL: This is the "time to live." This defines how many hops across the internet before the packet expires. It varies by the operating system making it helpful to identify the OS of the sender.

Protocol: This field defines what protocol is being used with IP. Most often, it will be 6 or TCP, 1 for ICMP, 17 for UDP, among others.

Header Checksum: This is an error-checking field. It calculates the checksum (a simple algorithm) to determine the integrity of the data in the header.


___________________



Rows 4 & 5

Source / Destination: These rows of the IP header are probably the most important part
of the header as it contains the source and destination IP address.
___________________

Row 6

Options: This field is variable in length, and its use is optional (as you might expect).
Padding: This field is used to fill out, if necessary, the remaining bits and bytes of the
header.

_____________________


# TCP (Transmission Control Protocol)



<img width="535" alt="Screenshot 2024-02-08 alle 16 18 11" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/e77c1d01-a5d6-4fa4-8630-e7d50fdfff3a">



Row 1
Source Port / Destination Port: Probably most importantly, these are the source port and destination port. These fields determine what port the communication came from (source) and where it is going (destination).

Row 2
Sequence Number: The sequence number is generated by the source machine's TCP stack and is used to make certain that packets are arranged in the proper sequence when they arrive. It is also important in defeating MitM attacks.

Row 3
Acknowledgment Number: 
Si tratta di un'eco del numero di sequenza inviato dal sistema ricevente. In pratica dice: "Ho ricevuto il pacchetto con il numero di sequenza". In questo modo, il mittente sa che il pacchetto è arrivato. Se il mittente non riceve un numero di conferma entro un determinato periodo di tempo, invia nuovamente il pacchetto per assicurarsi che il destinatario lo riceva. In questo modo, il TCP è affidabile (al contrario, l'UDP non lo fa ed è quindi inaffidabile).

Tralasciamo i bit CRW e ECE , i restanti 6 bit sono :


URG, ACK, PSH, RST, SYN, and FIN flags
These flags are used by TCP to communicate;


URG (Urgent): Il flag Urgent indica che i dati contenuti nel pacchetto devono essere trattati come urgenti e processati immediatamente. Se questo flag è impostato, il campo “Urgent Pointer” nell’intestazione TCP è valido e indica dove finiscono i dati urgenti nel payload del segmento, permettendo al ricevitore di dare priorità a questi dati.

ACK (Acknowledgement): Il flag di Acknowledgement viene utilizzato per confermare la ricezione corretta dei segmenti TCP. Quando è impostato, il campo “Acknowledgment Number” nell’intestazione è valido e indica il numero di sequenza del prossimo segmento che il mittente si aspetta di ricevere. Il flag ACK è quasi sempre attivo durante una connessione TCP a eccezione del primo segmento inviato dal mittente, che è identificato dal flag SYN.


PSH (Push): Il flag PSH, quando impostato, informa il ricevitore che i dati devono essere inoltrati all’applicazione immediatamente senza attendere il completamento del buffer. Ciò consente di trasferire dati rapidamente tra le applicazioni.


RST (Reset): Il flag Reset viene utilizzato per resettare una connessione. Se un host riceve un segmento che non è atteso o non è in grado di gestire, può inviare un segmento con il flag RST impostato per forzare la terminazione della connessione. Il flag RST può anche essere utilizzato per rifiutare tentativi di connessione non validi o per chiudere connessioni che sono diventate problematiche.



SYN (Synchronize): Il flag SYN viene utilizzato per stabilire una connessione TCP tra due host. Durante la fase di apertura della connessione TCP, conosciuta come handshake a tre vie, l’host che inizia la connessione invia un segmento con il flag SYN impostato per sincronizzare i numeri di sequenza tra i due endpoint.

FIN (Finish): Il flag FIN viene utilizzato per chiudere una connessione TCP. Un host invia un segmento con il flag FIN impostato per indicare che ha finito di inviare dati e vuole terminare la connessione. Dopo la ricezione del segmento FIN, l’altro endpoint conferma la richiesta di chiusura con un segmento ACK e può a sua volta inviare un FIN per chiudere la connessione da entrambe le parti.

<b> Nota </b>

Utilizzano nmap e creando pacchetti con combinazioni di flag che non dovrebbero essere viste in natura, potremmo essere in grado di suscitare 
una risposta da un sistema molto sicuro o addirittura di eludere il rilevamento.

Dimensione della finestra: In alcuni diagrammi è descritto semplicemente come campo Window. Il suo ruolo è quello di comunicare la dimensione della finestra che lo stack TCP ha per bufferizzare i pacchetti. È il modo in cui il TCP gestisce il controllo di flusso. Dal punto di vista della ricognizione o della forensics, questo campo può essere sufficiente per identificare il sistema operativo che ha inviato il pacchetto. Questo campo varia da OS a OS e persino da service pack a service pack. Con queste informazioni, si può prevedere con circa l'80% di precisione il sistema operativo che ha inviato il pacchetto. 
_____________________________


Row 5

Checksum: This field uses a simple algorithm to check for errors. In essence, it is an integrity checker.
URG Pointer: This field points to the last byte of the sequence number of urgent data. The URG flag must be set in conjunction to activate this field.

Row 6

Options: Like the IP header, the TCP header has an options field to be used if necessary, and it is varying length.
Padding: The padding is necessary to bring the TCP header to a multiple of 32 bits.

__________________________________


Nmap (Network Mapper) è uno strumento di sicurezza della rete, utilizzato per eseguire la scansione delle porte, l’enumerazione delle reti e la rilevazione delle vulnerabilità. Ecco come si possono utilizzare le opzioni per eseguire scansioni specifiche che coinvolgono i flag TCP SYN, FIN, ACK, RST, URG, e PSH:

### Scansione SYN (Half-Open Scan)

La scansione SYN (o half-open scan) è un tipo comune di scansione Nmap che invia pacchetti SYN a un obiettivo per vedere come risponde:


nmap -sS [target]



Dove [target] può essere un indirizzo IP o un range di indirizzi IP, un nome di dominio, ecc.

### Scansione FIN

Un’altra forma di scansione stealth, la scansione FIN, invia pacchetti TCP con il flag FIN impostato per vedere come risponde il dispositivo di destinazione. Questo può essere utilizzato per sondare un sistema senza innescare log di connessioni complete sul target:


nmap -sF [target]



### Scansione ACK (Per verificare i filtri)

La scansione ACK può essere utilizzata per determinare se i pacchetti con il flag ACK passano attraverso un firewall e quindi mappare le regole di filtraggio:


nmap -sA [target]



### Scansione Window

Una scansione Window è simile alla scansione ACK ma controlla le variazioni nella lunghezza della finestra di congestione. Non è uno standard di Nmap, ma può essere realizzata con l’opzione --scanflags che verrà presto discussa.

### Scansione Maimon

Questa è una scansione che invia pacchetti con i flag FIN e ACK impostati, prendendo il nome dal ricercatore che ha scoperto che questo tipo di pacchetti può rivelare porte aperte:


nmap -sM [target]



### Scansione Null, FIN e Xmas

Nmap consente anche combinazioni di flag come quelli Null (nessun flag impostato), FIN o Xmas (FIN, PSH, URG):

- Scansione Null (nessun flag):


nmap -sN [target]



- Scansione Xmas (plant a christmas tree):


nmap -sX [target]



Le scansioni Null, FIN e Xmas possono essere efficaci contro sistemi che non rispettano la RFC 793 del TCP. Secondo la RFC, se questi pacchetti sono inviati a una porta chiusa, il sistema deve rispondere con un pacchetto RST; le porte aperte dovrebbero ignorare il pacchetto e non rispondere.

### Uso di --scanflags

Con l’opzione --scanflags, Nmap consente di personalizzare i flag da usare nei pacchetti TCP inviati. Questo permette una flessibilità significativa, potendo settare direttamente qualsiasi combinazione di flag SYN, ACK, FIN, RST, URG, PSH, ecc. Ad esempio, per impostare i flag SYN e URG, si può usare il seguente comando:


nmap --scanflags URGPSH [target]










________________________________

# TCP Three-Way Handshake

Every TCP connection starts with a 3-way handshake. The handshake begins with a client sending a packet with the SYN flag set saying, 
“Hello, I want to talk to you” the server responds with a packet with the SYN and ACK flags set saying, “Hi, I’m willing and able to chat,” and
then finally, the client sends a packet with the ACK flag set that acknowledges the response of the server, and then the data transfer can begin.



<img width="460" alt="Screenshot 2024-02-08 alle 16 46 47" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/7c448fbf-8089-45bd-bc55-2e81c2cb4537">




Il TCP Three-Way Handshake è un processo utilizzato nel protocollo TCP (Transmission Control Protocol) per stabilire una connessione affidabile tra client e server su una rete basata su IP. Questa procedura è essenziale per garantire che entrambi gli endpoint siano pronti per iniziare la comunicazione e siano consapevoli della presenza l’uno dell’altro. Il three-way handshake si compone di tre fasi o passaggi:

### 1. SYN (Synchronize)

Il client inizia il processo inviando un segmento TCP al server in cui il flag SYN (synchronize sequence number) è impostato a 1, indicando il desiderio di stabilire una connessione. Questo segmento contiene anche un numero di sequenza iniziale (ISN), che è usato per tenere traccia dei byte trasferiti e assicurare l’ordine corretto dei dati all’arrivo.

- Client --> SYN=1, Seq=X --> Server

Il numero Seq=X rappresenta il numero di sequenza iniziale del client.

### 2. SYN-ACK (Synchronize-Acknowledgment)

Il server riceve il pacchetto SYN del client, processo che indica che il client è pronto per la comunicazione. Il server risponde inviando al client un segmento che ha sia il flag SYN che il flag ACK (acknowledgment) impostati a 1. Il numero di sequenza del server sarà un altro numero iniziale generato casualmente, e il numero di riconoscimento (ACK number) sarà incrementato di 1 rispetto al numero di sequenza iniziale del client, per riconoscere la ricezione del SYN del client.

- Server --> SYN=1, ACK=1, Seq=Y, Ack=X+1 --> Client

Il numero Seq=Y rappresenta il numero di sequenza iniziale del server e Ack=X+1 rappresenta la conferma della ricezione del SYN del client, indicando che il prossimo byte che il server si aspetta di ricevere dal client dovrebbe iniziare con il numero di sequenza X+1.

### 3. ACK (Acknowledgment)

Infine, il client invia un ulteriore segmento al server con il flag ACK impostato a 1 per confermare di aver ricevuto il segmento SYN-ACK del server. A questo punto, entrambi hanno riconosciuto i numeri di sequenza di partenza e confermato la disponibilità alla comunicazione.

- Client --> ACK=1, Seq=X+1, Ack=Y+1 --> Server

Il client incrementa l’ACK number a Y+1 per riconoscere di aver ricevuto il SYN dal server con il numero di sequenza Y.

Al termine di questo processo, la connessione TCP è considerata stabilita, e sia il client che il server possono iniziare la trasmissione dei dati. Ciò che rende il TCP affidabile è questa conferma esplicita dei numeri di sequenza e dei riconoscimenti prima che i dati effettivi vengano trasferiti. Ogni pacchetto di dati successivamente inviato su una connessione TCP è individuato da un numero di sequenza e richiede un riconoscimento dal destinatario, assicurando che nessun byte venga perso o duplicato durante la trasmissione.

______



# UDP


User Datagram Protocol o UDP è un protocollo senza connessione (rispetto a TCP, che è orientato alla connessione e richiede una connessione come l'handshake a 3 vie visto sopra). È più leggero del TCP perché non ha l'overhead di assicurare una connessione e di assicurarsi che ogni pacchetto arrivi. UDP invia semplicemente i pacchetti e se ne dimentica. È un'ottima soluzione per le applicazioni in cui si desidera efficienza e nessun pacchetto è critico, come lo streaming di musica o video.
Alcuni dei principali protocolli che utilizzano UDP sono il DNS (solo per le query), SNMP per la gestione dei dispositivi di rete e NTP per la sincronizzazione dell'ora di rete.
Quando si esegue la scansione delle porte UDP con strumenti come nmap, può essere necessario un po' più di tempo poiché UDP non prevede una risposta per i pacchetti persi o le porte chiuse. Nmap attende semplicemente un tempo specifico e, se non viene restituita alcuna risposta, presume che la porta sia chiusa. È possibile eseguire una scansione UDP con nmap con il seguente comando
kali > nmap -sU <indirizzo IP>



# Network Topologies



Quando i dispositivi sono collegati tra loro, esistono diverse opzioni per la disposizione fisica dei dispositivi. Questa disposizione fisica può essere molto importante per ottimizzare la distanza, la latenza, la congestione e la disponibilità di due nodi della rete. Questa configurazione fisica è nota come topologia.



<b>Star Topology</b>


La topologia a stella è la topologia più diffusa per le reti locali (LAN). Nella topologia a stella, c'è un server al centro della stella e tutti i client si collegano al server. Il vantaggio di questa topologia è che le connessioni di ciascun client sono indipendenti e se un client o la sua connessione si interrompe, gli altri client possono comunque comunicare con il server.


<img width="482" alt="Screenshot 2024-02-10 alle 13 19 59" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/804cd2d1-6e73-4f7b-bc94-2434a8fbdd6a">

<b>Ring topology </b>
La topologia ad anello invia i pacchetti intorno a un anello e solo il client a cui è destinato il pacchetto può prenderlo dall'anello. Il vantaggio della topologia ad anello è che è semplice e poco costosa, ma se l'anello si rompe, tutti i client non possono ricevere alcuna comunicazione.




<img width="503" alt="Screenshot 2024-02-10 alle 13 23 46" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/1c111a91-5baa-48d4-9c2c-8600ae9fe8ca">



<b>Mesh Topology</b>


La topologia mesh prevede molte connessioni tra ogni dispositivo della rete. Ciò significa che un pacchetto ha diversi percorsi per arrivare a destinazione. Ciò conferisce alla rete una certa resilienza nel caso in cui un cavo o un percorso sia interrotto. Questo è simile al modo in cui è connessa la nostra moderna Internet: i pacchetti hanno più percorsi da seguire per raggiungere il sistema di destinazione. 


___________________________________________________________________


# The OSI Model


I modelli OSI e TCP sono i più comuni per comprendere il modo in cui i vari protocolli lavorano insieme. 
Cominciamo con il modello OSI. Il diagramma seguente mostra i sette livelli e l'uso di base di tale livello nella comunicazione di rete.


<img width="517" alt="Screenshot 2024-02-10 alle 13 29 28" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/867ec6e1-f9d6-41c1-9571-bb163d94478f">


Come si può notare, il modello OSI comprende sette livelli: il livello Applicazione, il livello Presentazione, il livello Sessione, il livello Trasporto, il livello Rete, il livello Collegamento dati e infine il livello Fisico. La figura precedente illustra in dettaglio i vari livelli e i protocolli e le attività associate a ciascuno di essi. Per aiutare a ricordare i vari livelli di questo modello, esistono almeno due dispositivi mnemonici. Se partiamo dall'alto e scendiamo verso il basso, possiamo prendere la prima lettera di ogni livello, ovvero A, P, S, T, N, D e P. Molte persone ricordano questi livelli utilizzando questo dispositivo mnemonico;

All People Seem To Need Data Processing




# The OSI Model from a Cybersecurity Perspective


<img width="461" alt="Screenshot 2024-02-10 alle 13 32 45" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/417bb9bb-c7f2-42d3-b211-529ebf07f3b6">


Il livello Applicazione comprende generalmente applicazioni come browser, word processor e altre applicazioni. Gli attacchi più importanti di questo livello sono probabilmente gli exploit. Si tratta di attacchi che spesso possono incorporare il codice dell'hacker all'interno dell'applicazione per prendere il controllo dell'applicazione e del sistema.
Al livello Presentazione, l'attacco più preoccupante è il phishing o l'invio di e-mail a varie persone con link dannosi.
A livello di sessione, l'attacco più importante è l'hijacking. L'hijacking consiste nel fatto che un aggressore può appropriarsi di una sessione esistente stabilita legittimamente dall'utente.
Al livello Trasporto, l'hacker spesso effettua la sua ricognizione a questo livello.
A livello di rete, gli aggressori possono condurre attacchi Man-in-the-Middle MiTM) in cui si interpongono tra un utente legittimo e un server, intercettando il traffico ed eventualmente alterandolo.


Al livello Data Link, l'aggressore può falsificare gli indirizzi MAC, l'indirizzo univoco globale impresso su ogni dispositivo collegato in rete ed essenziale per il corretto funzionamento di una LAN (vedere ARP).
Infine, il livello fisico può essere attaccato con lo sniffing. Lo sniffing è la pratica di osservare e analizzare il traffico di rete (vedere Wireshark e Sniffer).


_______________________________________________



# SUBNETTING



Il subnetting è una tecnica utilizzata nella progettazione delle reti per suddividere una rete IP più grande in sotto-reti più piccole. Questo processo consente di ottimizzare l'utilizzo degli indirizzi IP disponibili e di migliorare l'efficienza della rete. In sostanza, il subnetting consente di dividere un blocco di indirizzi IP in porzioni più gestibili e organizzate.
il subnetting è una pratica importante nella progettazione delle reti per ottimizzare l'uso degli indirizzi IP e migliorare l'efficienza complessiva della rete.


Indirizzi IP: Un indirizzo IP è un identificatore univoco assegnato a ogni dispositivo in una rete che utilizza il protocollo Internet (IP). Gli indirizzi IP sono formati da numeri decimali separati da punti (ad esempio, 192.168.1.1).

Maschera di sottorete (subnet mask): La maschera di sottorete determina quale parte di un indirizzo IP è dedicata alla rete e quale parte è riservata agli host nella rete. È rappresentata da una serie di bit a 1 seguiti da una serie di bit a 0. Ad esempio, in una maschera di sottorete 255.255.255.0, i primi 24 bit sono dedicati alla rete e gli ultimi 8 bit sono riservati agli host.

Suddivisione delle reti: Utilizzando il subnetting, è possibile suddividere una rete più grande in sotto-reti più piccole. Ad esempio, se si ha un blocco di indirizzi IP come 192.168.1.0 con una maschera di sottorete 255.255.255.0, è possibile suddividere questa rete in sotto-reti più piccole.

 CIDR (Classless Inter-Domain Routing): CIDR è un metodo di rappresentazione degli indirizzi IP e delle loro lunghezze di prefisso. Ad esempio, anziché usare una maschera di sottorete come 255.255.255.0, si potrebbe rappresentare la stessa informazione come /24. Questo indica che i primi 24 bit dell'indirizzo IP sono riservati alla rete.

Numero di host e sottoreti: Suddividendo una rete in sotto-reti più piccole, è possibile avere più sottoreti con un numero specifico di host. Questo può essere utile per ottimizzare l'allocazione degli indirizzi IP e migliorare le prestazioni della rete.


<img width="511" alt="Screenshot 2024-02-10 alle 13 43 51" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/0924b433-5ea5-4429-b4b0-cd5b6789ebaa">



<img width="672" alt="Screenshot 2024-02-10 alle 13 57 36" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/75343b14-c69f-4b97-a259-52d88867996d">

____________________________


<b> Indirizzo di broadcast </b>

L'indirizzo di broadcast è un indirizzo speciale utilizzato nelle reti per inviare un messaggio a tutti gli host presenti nella stessa rete. Quando un dispositivo invia un pacchetto alla direzione di broadcast, ogni host nella rete riceverà e processerà il messaggio. Questo è utile, ad esempio, quando si desidera inviare un messaggio a tutti gli host in una rete, come un annuncio o una richiesta di risorse.

L'indirizzo di broadcast varia a seconda della classe di indirizzo IP e della maschera di sottorete utilizzata. In una rete IPv4, l'indirizzo di broadcast è spesso l'indirizzo in cui tutti i bit riservati agli host sono impostati su 1. Ad esempio, in una rete con l'indirizzo IP 192.168.1.0 e una maschera di sottorete di 255.255.255.0, l'indirizzo di broadcast sarà 192.168.1.255.

Nel contesto delle reti IPv6, non esiste un vero e proprio indirizzo di broadcast, ma viene utilizzato l'indirizzo multicast speciale "ff02::1", noto come "All Nodes Address". Gli host IPv6 interessati ascolteranno i pacchetti inviati a questo indirizzo multicast.


> comando ipcalc


<b> Indirizzo di loopback </b>


L'indirizzo di loopback è un indirizzo speciale utilizzato per testare la connettività di una scheda di rete o per accedere ai servizi locali su un computer senza dover attraversare una rete fisica. Questo indirizzo consente di inviare pacchetti a se stessi, senza che essi lascino effettivamente la scheda di rete.

In IPv4, l'indirizzo di loopback è 127.0.0.1. Può essere usato per accedere a servizi locali, come server web o database, senza doverli instradare attraverso una rete fisica. Ad esempio, digitando "http://127.0.0.1" nella barra degli indirizzi del browser, si accede al server web in esecuzione sulla stessa macchina.

In IPv6, l'equivalente dell'indirizzo di loopback è "::1".

L'utilizzo dell'indirizzo di loopback è particolarmente utile durante lo sviluppo e il debug di applicazioni di rete, in quanto consente di testare la funzionalità di rete senza dipendere da una connessione di rete effettiva.



<b> Indirizzi riservati </b>


Gli indirizzi riservati sono blocchi specifici di indirizzi IP assegnati per scopi speciali o interni e non sono utilizzabili su Internet pubblico. Questi indirizzi sono riservati per garantire che siano utilizzati in modo coerente e prevenire conflitti di indirizzamento. Alcuni esempi di indirizzi riservati includono:

1. **Indirizzi privati IPv4**: Questi indirizzi sono assegnati per l'uso all'interno di reti private e non sono indirizzi IP pubblici. I tre blocchi principali sono:
   - 10.0.0.0 a 10.255.255.255 (classe A)
   - 172.16.0.0 a 172.31.255.255 (classe B)
   - 192.168.0.0 a 192.168.255.255 (classe C)

2. **Indirizzo di loopback IPv4**: 127.0.0.1 è riservato per scopi di loopback, permettendo a un dispositivo di inviare pacchetti a se stesso.

3. **Indirizzi di loopback IPv6**: ::1 è l'equivalente di loopback per IPv6.

4. **Indirizzi di documentazione IPv4 e IPv6**: Questi indirizzi sono utilizzati per scopi di documentazione e non dovrebbero essere utilizzati in reti operative. Ad esempio, 192.0.2.0 è un blocco riservato per esempi di documentazione.

5. **Indirizzi multicast**: Alcuni blocchi di indirizzi sono riservati per l'uso multicast, come il blocco IPv4 224.0.0.0 a 239.255.255.255.

6. **Indirizzi link-local IPv6**: Gli indirizzi IPv6 che iniziano con "fe80::" sono riservati per l'uso link-local, ovvero per comunicazioni su una singola rete locale.

L'uso degli indirizzi riservati è una pratica importante per garantire la stabilità e la sicurezza delle reti, evitando conflitti di indirizzamento e garantendo la corretta operatività delle comunicazioni in ambienti specifici.


_____________________________________________


```
> ipcalc 192.168.1.7 /16
```

Siccome l'indirizzo è a 32 bit -> 8 bit -> 192 , 168 -> 8 bit  ecc

/ 16 significa che per indicare la rete uso 192.168 , mentre la restante parte mi identifica l'host

totale degli host ho 65536 - 2 ( indirizzo di broadcast e nome della rete  )


Cosa succede se faccio ?
```
> ipcalc 192.168.1.7 /25
```

CIDR NOTATION.

CIDR, o Classless Inter-Domain Routing notation, è un modo di rappresentare un indirizzo IP e la maschera di rete ad esso associata. La notazione CIDR specifica un indirizzo IP, una barra (/) e un numero decimale come 192.168.1.0/24, dove il 24 rappresenta il numero di bit della maschera di rete. Naturalmente, il numero di bit può variare a seconda del numero di sottoreti.



# NETWORK ANALYSIS


<img width="595" alt="Screenshot 2024-02-10 alle 14 53 19" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/b0f4d3b8-919e-43fa-8dba-2f94686cf876">




Comando ping


Il comando ping è una utilità di rete comune utilizzata per testare la connettività tra due dispositivi su una rete IP

```
ping hackers-arise.com
```



Alcuni comuni parametri aggiuntivi del comando ping includono:

    -c: Specifica il numero di pacchetti da inviare. Ad esempio, -c 4 invierà 4 pacchetti.
    -i: Specifica l'intervallo di tempo tra l'invio di ogni pacchetto.
    -t (solo su Windows): Pinga continuamente il dispositivo di destinazione fino a quando viene interrotto manualmente.

Ad esempio:



bash
```
ping -c 4 -i 1 192.168.1.1
```
Questo invierà 4 pacchetti a 192.168.1.1 con un intervallo di 1 secondo tra ciascun pacchetto.



Il comando `netstat` è un'utilità di rete disponibile su molti sistemi operativi, inclusi Linux, Windows e macOS. Esso fornisce informazioni dettagliate sullo stato delle connessioni di rete, delle interfacce di rete, delle tabelle di routing, dei servizi in ascolto e altro ancora. L'output specifico può variare a seconda del sistema operativo e delle opzioni specificate.


This can help with monitoring and troubleshooting network connections. In some cases, I have used it to find malware connecting to my system.

Ecco alcuni esempi di come utilizzare il comando `netstat`:

1. **Visualizzare tutte le connessioni di rete:**
   ```bash
   netstat -a
   ```
   Questo comando mostra tutte le connessioni di rete, sia in ascolto che in stato di established.

2. **Visualizzare le connessioni di rete con informazioni dettagliate:**
   ```bash
   netstat -an
   ```
   Questo comando mostra le connessioni di rete con dettagli come indirizzo IP e numero di porta.

3. **Visualizzare le statistiche delle interfacce di rete:**
   ```bash
   netstat -i
   ```
   Questo comando fornisce statistiche dettagliate sulle interfacce di rete, inclusi pacchetti trasmessi e ricevuti.

4. **Visualizzare le tabelle di routing:**
   ```bash
   netstat -r
   ```
   Questo comando mostra le tabelle di routing del sistema.

5. **Visualizzare i servizi in ascolto:**
   ```bash
   netstat -l
   ```
   Questo comando mostra i servizi in ascolto sul sistema.

6. **Visualizzare le connessioni di rete usando un determinato protocollo (es. TCP):**
   ```bash
   netstat -at
   ```
   Questo comando mostra solo le connessioni di tipo TCP.

7. **Visualizzare le connessioni di rete in tempo reale (monitoraggio continuo):**
   ```bash
   netstat -c
   ```
   Questo comando aggiorna continuamente l'output, mostrando le connessioni di rete in tempo reale.



Ulteriori comandi :

Visualizzare tutte le connessioni tcp
```
> netstat -t 
```

Visualizzare tutte le connessioni udp

```
> netstat -u 
```

Visualizzare tutte le connessioni 
```
> netstat -l 
```


If you have an Apache or nginx web server running on your system listening for connections, you can check by piping netstat –a to grep http, such as
```
netstat –a | grep http
```


### comando ss

Il comando `ss` è un'utilità di sistema utilizzata per visualizzare informazioni dettagliate sulle connessioni di rete, le interfacce di rete, i socket e altro ancora su sistemi Linux e UNIX-like. È spesso considerato più avanzato e più efficiente rispetto al comando `netstat`.
(`man ss`) per ottenere ulteriori dettagli e opzioni specifiche del sistema.



 **Visualizzare tutte le connessioni di rete:**
   ```bash
   ss
   ```
   Questo comando mostra tutte le connessioni di rete, inclusi i dettagli come indirizzo IP, numero di porta, stato e altro ancora.

**Visualizzare le connessioni di rete in formato esteso:**
   ```bash
   ss -e
   ```
   Mostra informazioni estese, inclusi i dettagli dei processi associati alle connessioni.

 **Visualizzare le connessioni di rete in formato numerico:**
   ```bash
   ss -n
   ```
   Visualizza le connessioni di rete in formato numerico senza risolvere gli indirizzi o i nomi di servizio.

**Visualizzare solo le connessioni di tipo TCP:**
   ```bash
   ss -t
   ```
   Mostra solo le connessioni di tipo TCP.

 **Visualizzare solo le connessioni di tipo UDP:**
   ```bash
   ss -u
   ```
   Mostra solo le connessioni di tipo UDP.

**Visualizzare le statistiche sulle interfacce di rete:**
   ```bash
   ss -s
   ```
   Mostra statistiche sulle interfacce di rete, inclusi pacchetti trasmessi e ricevuti.

 **Visualizzare i servizi in ascolto:**
   ```bash
   ss -l
   ```
   Mostra i servizi in ascolto sul sistema.

**Visualizzare le connessioni di rete in tempo reale (monitoraggio continuo):**
   ```bash
   watch -n 1 ss
   ```
   Utilizza il comando `watch` per aggiornare continuamente l'output del comando `ss` ogni secondo.


### NETWORK SNIFFERS


A network sniffer—sometimes referred to as a packet analyzer, protocol analyzer, or network traffic analyzer—can intercept and analyze network traffic that traverses a digital network. These sniffers can be invaluable to the network or security engineer, the forensic investigator, and in some cases, the hacker. For instance, if an application sends passwords over the network unencrypted, the hacker may be able to sniff and view the passwords. Since only a few applications send passwords unencrypted in our security-conscious era, the value of the sniffer to the hacker is a bit more nuanced.
For some exploits/hacks, such as DNS or MiTM attacks, analysis of the LAN traffic can be crucial to their success, making the sniffer invaluable. Besides, sniffing a target’s traffic can reveal what sites they are visiting, their cookies, their user agent, or even their email messages (if unencrypted or you have the resources to decrypt the message).
Many tools are capable of network sniffing, including:

1. SolarWinds Deep Packet Inspection and Analysis Tool
2. Tcpdump
3. Windump
4. Wireshark
5. Network Miner
6. Capsa
7. tshark



<b>Prerequisiti per lo sniffing</b>
È fondamentale sottolineare che per utilizzare efficacemente uno sniffer di rete, la scheda di interfaccia di rete (NIC) deve essere in modalità promiscua. Ciò significa che la scheda NIC rileva QUALSIASI pacchetto che attraversa la rete. Di solito, le schede NIC raccolgono solo i pacchetti destinati al loro particolare indirizzo MAC (Globally Unique Physical).
L'altro punto critico da comprendere con lo sniffing di rete è che il formato di file standard per lo sniffing è .pcap (packet capture). Ciò significa che il vostro sistema deve avere una libreria (un po' di codice riutilizzabile) per mettere i pacchetti in questo formato. Queste librerie sono libpcap sul sistema Linux o Winpcap sul sistema Windows.


**tcpdump in Action**


Il comando `tcpdump` è uno strumento di cattura dei pacchetti di rete disponibile su sistemi operativi UNIX-like, inclusi Linux e macOS. Esso consente di catturare e analizzare il traffico di rete in tempo reale. `tcpdump` offre una vasta gamma di opzioni per filtrare, visualizzare e analizzare i pacchetti di rete. Di solito, è necessario avere privilegi di amministratore (solitamente con `sudo`) per eseguire `tcpdump`.
(`man tcpdump`).


Esempi

 **Catturare tutto il traffico su una interfaccia di rete:**
   ```bash
   sudo tcpdump -i interfaccia
   ```
   Sostituisci "interfaccia" con il nome della tua interfaccia di rete (ad esempio, eth0).

 **Catturare solo il traffico TCP:**
   ```bash
   sudo tcpdump -i interfaccia tcp
   ```

**Catturare il traffico su una specifica porta:**
   ```bash
   sudo tcpdump -i interfaccia port numero_porta
   ```
   Sostituisci "numero_porta" con il numero della porta desiderata.

**Catturare il traffico su un indirizzo IP specifico:**
   ```bash
   sudo tcpdump -i interfaccia host indirizzo_ip
   ```
   Sostituisci "indirizzo_ip" con l'indirizzo IP desiderato.

**Catturare il traffico su una rete o sottorete specifica:**
   ```bash
   sudo tcpdump -i interfaccia net indirizzo_rete/maschera_sottorete
   ```

**Visualizzare dettagli in formato leggibile:**
   ```bash
   sudo tcpdump -i interfaccia -A
   ```
   Questo comando visualizza il contenuto dei pacchetti in formato testo.

**Salvare la cattura su un file per l'analisi successiva:**
   ```bash
   sudo tcpdump -i interfaccia -w nome_file
   ```
   Questo salverà i pacchetti catturati in un file binario.

**Leggere un file di cattura esistente:**
   ```bash
   sudo tcpdump -r nome_file
   ```
   Questo leggerà un file di cattura esistente.


<img width="1413" alt="Screenshot 2024-02-10 alle 15 20 03" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/3352f0b7-fe0a-4e38-8b1d-81b382c61895">


<img width="1233" alt="Screenshot 2024-02-10 alle 15 20 21" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/c89e5447-8fc6-422f-84fc-2d66354ec78f">

```
tcpdump src host 192.168.0.114
```
Questo comando visualizzerà i pacchetti in arrivo o in partenza dall'host con indirizzo IP 192.168.0.114 sulla rete a cui è connesso l'interfaccia di rete specificata. 



```
tcpdump –vv dst port 80
```


-vv: Aumenta il livello di dettaglio dell'output di tcpdump. L'opzione -vv mostra più informazioni sulle intestazioni dei pacchetti, inclusi dettagli specifici sul protocollo e altri dettagli.

dst port 80: Specifica un filtro sui pacchetti da catturare. Questo filtro indica di catturare solo i pacchetti in cui la porta di destinazione è 80. La porta 80 è comunemente associata ai servizi HTTP, quindi questo filtro cattura il traffico destinato ai server web.




**Filter by TCP Flags**
What if we wanted to see only the traffic with SYN flags sets on it? We could create a filter like this:
```
tcpdump ‘tcp[tcpflags]==tcp-syn’
```

Altri esempi di regole :


kali > tcpdump ‘tcp[tcpflags]==tcp-ack’
kali > tcpdump ‘tcp[tcpflags]==tcp-fin’ 
kali > tcpdump ‘tcp[tcpflags]==tcp-rst’ 
kali > tcpdump ‘tcp[tcpflags]==tcp-psh’ 
kali > tcpdump ‘tcp[tcpflags]==tcp-urg’



**Combining Filters**

tcpdump enables us to use filters together using a logical AND (&&) or a logical OR (||). So, if we wanted to filter for a particular IP address and TCP port 80 we would create a filter such as:
```
tcpdump host 192.168.0.114 and port 80
```
We can also use a logical OR, such as: 
```
tcpdump port 80 or port 443
```
If we want to see all the traffic except that traveling from a particular IP address, we can use the negation symbol (!) or not.
```
tcpdump not host 192.168.0.114
```



**Filtering for Passwords and Identifying Artifacts**

To filter for passwords in cleartext, we could build a filter for various ports and then use egrep to search for strings indicating logins or passwords.
```
tcpdump port 80 or port 21 or port 25 or port 110 or port 143 or port 23 –lA | egrep –i B5 ‘pass=|pwd=|log=|login=|user=|username=|pw=|passw=|password=’
```

Finally, if you want to filter for just the user agent (an identifying signature of the user and their browser) we could create a filter such as:
```
tcpdump –vvAls | grep ‘User-Agent’

```


Finally, to filter for just the browser cookies, we can create the following filter.
```
tcpdump –vvAls | grep ‘Set-Cookie|Host|Cookie:’
```


_____________________________________________________________________________________________________________

### Wireshark

Wireshark è un popolare analizzatore di protocolli di rete open-source. Questo strumento consente di catturare e analizzare il traffico di rete in tempo reale. Wireshark supporta una vasta gamma di protocolli di rete ed è disponibile per diverse piattaforme, inclusi Windows, Linux e macOS.

Cosa posso fare con Wireshark:

**Cattura dei pacchetti:** Wireshark permette di catturare pacchetti di dati in tempo reale da una interfaccia di rete specifica.

**Filtraggio avanzato:** Offre potenti opzioni di filtraggio per visualizzare solo i pacchetti di interesse. I filtri possono essere applicati in base a criteri come indirizzi IP, protocolli, porte e altro ancora.

**Analisi di protocollo:** Wireshark decodifica automaticamente numerosi protocolli di rete e visualizza chiaramente le informazioni contenute nei pacchetti. Può mostrare i dettagli dei protocolli di livello applicativo come HTTP, DNS, TCP, UDP e molti altri.

**Analisi dei flussi:** Wireshark offre funzionalità per seguire i flussi di comunicazione tra gli host, facilitando la comprensione delle interazioni complesse tra i dispositivi di rete.

**Colorazione dei pacchetti:** I pacchetti vengono colorati in base ai criteri definiti, rendendo più facile identificare e distinguere diversi tipi di pacchetti.

**Esportazione dei dati:** È possibile esportare i dati catturati in vari formati, come file di tipo CSV o JSON, per ulteriori analisi.

**Supporto per diversi formati di cattura:** Wireshark supporta una vasta gamma di formati di file di cattura, inclusi quelli generati da altre utilità come tcpdump.




<img width="487" alt="Screenshot 2024-02-11 alle 10 47 11" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/e5ba32ae-9071-4d37-a4bb-4355fdf178bc">


In Wireshark sono presenti tre finestre di analisi separate. La finestra superiore, contrassegnata con il numero 1 nell'immagine soprastante, è nota come riquadro dell'elenco dei pacchetti. In questa finestra si vedono i pacchetti codificati a colori che si muovono in tempo reale.


La finestra centrale, denominata #2, è nota come riquadro dei dettagli del pacchetto. Questo riquadro fornisce le informazioni sull'intestazione del pacchetto selezionato nella finestra #1.


Infine, la finestra n. 3, riquadro Bytes del pacchetto, fornisce informazioni sul carico utile sia in formato esadecimale a sinistra che in formato ASCII a destra.


**APPLICAZIONE DEI FILTRI**

<img width="1187" alt="Screenshot 2024-02-11 alle 10 51 41" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/2f307a1a-e992-4e3b-b17d-55403051a5af">



Wireshark offre un potente meccanismo di filtraggio consente di concentrarsi sui pacchetti di interesse durante l'analisi del traffico di rete. I filtri possono essere applicati attraverso la barra degli strumenti di Wireshark o attraverso la finestra di filtro.



VEDI DOCUMENTAZIONE : https://wiki.wireshark.org/DisplayFilters

 **Filtri per indirizzo IP:**
   - Filtra i pacchetti con un indirizzo IP sorgente specifico: `ip.src == 192.168.1.1`
   - Filtra i pacchetti con un indirizzo IP di destinazione specifico: `ip.dst == 192.168.1.1`
   - Filtra i pacchetti tra due indirizzi IP: `ip.addr == 192.168.1.1`

 **Filtri per protocollo:**
   - Filtra i pacchetti HTTP: `http`
   - Filtra i pacchetti DNS: `dns`
   - Filtra i pacchetti TCP: `tcp`
   - Filtra i pacchetti UDP: `udp`

**Filtri per porta:**
   - Filtra i pacchetti con una porta sorgente specifica: `tcp.srcport == 80`
   - Filtra i pacchetti con una porta di destinazione specifica: `tcp.dstport == 443`
   - Filtra i pacchetti con una porta specifica (sorgente o destinazione): `tcp.port == 22`

**Filtri logici:**
   - Filtra i pacchetti che soddisfano entrambe le condizioni: `ip.src == 192.168.1.1 && tcp.port == 80`
   - Filtra i pacchetti che soddisfano una delle condizioni: `ip.src == 192.168.1.1 || ip.dst == 192.168.1.2`

**Filtri per dati specifici:**
   - Filtra i pacchetti contenenti una stringa specifica nei dati (payload): `data contains "parola_chiave"`
   - Altro esempio : tcp contains facebook

**Filtri per lunghezza dei pacchetti:**
   - Filtra i pacchetti con una lunghezza minima specifica: `frame.len >= 100`
   - Filtra i pacchetti con una lunghezza massima specifica: `frame.len <= 500`



____________________________________________________________________________________________________




# Linux Firewalls


Def :

A firewall is a subsystem on a computer that blocks certain network traffic from going into or out of a computer. Firewalls can be either software or hardware-based. Hardware-based firewalls generally are used to protect a network and the computers on it, while a software-based firewall protects the system hosting it.

![Screenshot 2024-02-11 alle 11 00 01](https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/87b9d25c-af8d-48f3-9ee9-c670369c07e5)




**IPTABLES**

```
sudo apt install iptables
```
documentazione ufficiale (`man iptables`)

`iptables` è un'utilità di filtraggio del pacchetto e di gestione del firewall per i sistemi basati su Linux. Consente agli amministratori di sistema di definire regole per il filtraggio del traffico di rete, consentendo o negando il passaggio di pacchetti attraverso una interfaccia di rete. 

Cosa trovo in iptables :

 **Tabelle:**
   `iptables` organizza le regole in tabelle. Le tabelle principali sono:
   - `filter`: Utilizzata per il filtraggio del traffico.
   - `nat`: Utilizzata per la traduzione degli indirizzi di rete (Network Address Translation).
   - `mangle`: Utilizzata per la modifica di pacchetti.
   - `raw`: Utilizzata per regole che non dovrebbero essere modificate dalla conntrack.

 **Catene (Chains):**
   All'interno di ogni tabella, `iptables` contiene catene che rappresentano insiemi di regole. Le catene principali sono:
   - `INPUT`: Applica le regole al traffico in arrivo.
   - `OUTPUT`: Applica le regole al traffico in uscita.
   - `FORWARD`: Applica le regole al traffico di attraversamento (quando il sistema agisce da router).
   - Altre catene personalizzate possono essere create per organizzare le regole in modo più specifico.

**Regole:**
   Le regole definiscono come il traffico deve essere gestito. Ogni regola specifica un insieme di condizioni e un'azione da intraprendere se le condizioni sono soddisfatte. Le azioni comuni includono `ACCEPT` (accetta il pacchetto), `DROP` (scarta il pacchetto) e `REJECT` (scarta il pacchetto e invia un messaggio di errore al mittente).

**Target:**
   Il target è l'azione intrapresa quando una regola corrispondente viene trovata. Alcuni esempi di target includono `ACCEPT`, `DROP`, `REJECT`, `MASQUERADE` (nel caso della tabella `nat` per la NAT), ecc.

Ecco un esempio semplice di utilizzo di `iptables`:

```bash
# Pulisce le regole esistenti
sudo iptables -F

# Impedisce tutto il traffico in ingresso e in uscita
sudo iptables -P INPUT DROP
sudo iptables -P OUTPUT DROP

# Permette il traffico di loopback
sudo iptables -A INPUT -i lo -j ACCEPT
sudo iptables -A OUTPUT -o lo -j ACCEPT

# Permette il traffico SSH in ingresso
sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT
```

Questo esempio configura un firewall di base che consente solo il traffico di loopback e il traffico SSH in ingresso. È importante notare che queste regole saranno temporanee e saranno perse al riavvio del sistema a meno che non vengano salvate in modo permanente.

Per salvare le regole in modo permanente su sistemi basati su Debian/Ubuntu, è possibile utilizzare il comando:

```bash
sudo iptables-save > /etc/iptables/rules.v4
```


**ESERCITAZIONE**


**Esercizio 1: Introduzione a iptables**

Supponiamo di avere un server Linux con due interfacce di rete: `eth0` e `eth1`. Configura un set di regole iptables per consentire il traffico SSH in ingresso solo dalla sottorete `192.168.1.0/24` sull'interfaccia `eth0`.

**Soluzione:**
```bash
# Pulisce le regole esistenti
sudo iptables -F

# Imposta la policy predefinita a DROP
sudo iptables -P INPUT DROP
sudo iptables -P FORWARD DROP
sudo iptables -P OUTPUT ACCEPT

# Permette il traffico di loopback
sudo iptables -A INPUT -i lo -j ACCEPT
sudo iptables -A OUTPUT -o lo -j ACCEPT

# Permette il traffico SSH in ingresso dalla sottorete 192.168.1.0/24 sull'interfaccia eth0
sudo iptables -A INPUT -i eth0 -p tcp --dport 22 -s 192.168.1.0/24 -j ACCEPT
```

**Esercizio 2: Filtraggio avanzato con iptables**

Configura iptables per consentire il traffico HTTP in ingresso solo da un singolo indirizzo IP, bloccando tutto il resto del traffico in ingresso.

**Soluzione:**
```bash
# Pulisce le regole esistenti
sudo iptables -F

# Imposta la policy predefinita a DROP
sudo iptables -P INPUT DROP
sudo iptables -P FORWARD DROP
sudo iptables -P OUTPUT ACCEPT

# Permette il traffico di loopback
sudo iptables -A INPUT -i lo -j ACCEPT
sudo iptables -A OUTPUT -o lo -j ACCEPT

# Permette il traffico HTTP in ingresso solo da un indirizzo IP specifico
sudo iptables -A INPUT -p tcp --dport 80 -s indirizzo_ip_specifico -j ACCEPT
```

**Esercizio 3: Gestione delle connessioni con iptables**

Configura iptables per consentire il traffico SSH in ingresso da qualsiasi indirizzo IP, ma blocca il traffico SSH in uscita solo per un intervallo specifico di porte.

**Soluzione:**
```bash
# Pulisce le regole esistenti
sudo iptables -F

# Imposta la policy predefinita a DROP
sudo iptables -P INPUT DROP
sudo iptables -P FORWARD DROP
sudo iptables -P OUTPUT DROP

# Permette il traffico di loopback
sudo iptables -A INPUT -i lo -j ACCEPT
sudo iptables -A OUTPUT -o lo -j ACCEPT

# Permette il traffico SSH in ingresso da qualsiasi indirizzo IP
sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT

# Consente il traffico SSH in uscita solo per le porte 1024-65535
sudo iptables -A OUTPUT -p tcp --sport 22 --dport 1024:65535 -j ACCEPT
```


____________________________________________________


# ADDRESS RESOLUTION PROTOCOL  ( ARP ) 


<img width="410" alt="Screenshot 2024-02-11 alle 11 10 09" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/fce08f7b-0f23-4604-84f4-72ea5a30aead">



Il Protocollo di Risoluzione degli Indirizzi (ARP - Address Resolution Protocol) è un protocollo di rete utilizzato per associare un indirizzo IP a un indirizzo MAC (Media Access Control) su una rete locale.
Il suo scopo principale è tradurre gli indirizzi di rete livello 3 (come gli indirizzi IP) negli indirizzi fisici a livello 2 (come gli indirizzi MAC).

**Quando è utilizzato ?**

È utilizzato nella fase di inizializzazione della comunicazione tra dispositivi sulla stessa rete locale, garantendo che i pacchetti possano essere correttamente instradati a livello di collegamento dati.

**Caching**
La cache ARP è temporanea e può essere aggiornata o cancellata nel tempo. Ad esempio, quando i dispositivi si spengono o vengono disconnessi dalla rete, le voci corrispondenti nella cache ARP possono essere eliminate.

**COME FUNZIONA ?**

Richiesta ARP (ARP Request):
Quando un dispositivo sulla rete desidera inviare un pacchetto a un altro dispositivo, ma conosce solo il suo indirizzo IP, invia una richiesta ARP broadcast. Questa richiesta contiene l'indirizzo IP del dispositivo di destinazione e chiede quale sia il suo indirizzo MAC. La richiesta è inviata a tutti i dispositivi sulla stessa rete locale.

Risposta ARP (ARP Reply):
Il dispositivo di destinazione, che riconosce il proprio indirizzo IP nella richiesta ARP, risponde inviando un pacchetto ARP contenente il suo indirizzo MAC. Questa risposta è inviata direttamente al dispositivo che ha iniziato la richiesta ARP.

Memorizzazione nella Cache ARP:
I dispositivi coinvolti memorizzano le informazioni ottenute nel processo ARP in una tabella nota come "cache ARP" o "tabella ARP". Questa tabella tiene traccia delle associazioni tra indirizzi IP e indirizzi MAC per ridurre la necessità di nuove richieste ARP per lo stesso dispositivo sulla rete.


**APPROFONDIMENTO SU CACHE ARP**

La cache ARP, anche conosciuta come "tabella ARP", è una memoria temporanea che contiene le associazioni tra gli indirizzi IP e gli indirizzi MAC sulla rete locale di un dispositivo. La posizione specifica della cache ARP può variare a seconda del sistema operativo.


**Sistemi operativi basati su Linux:**
   - Su sistemi Linux, la cache ARP è memorizzata nel kernel e può essere visualizzata utilizzando il comando `arp`.
   - La posizione del file che memorizza le informazioni sulla cache ARP varia tra le distribuzioni Linux. In molte distribuzioni, queste informazioni sono temporanee e gestite direttamente dal kernel.

**Sistemi operativi basati su Windows:**
   - Su sistemi Windows, la cache ARP è memorizzata nel Registro di sistema e può essere visualizzata utilizzando il comando `arp`.
   - La cache ARP su Windows è anche temporanea e viene gestita dal sistema operativo.

**Sistemi operativi basati su macOS:**
   - Su macOS (precedentemente noto come OS X), la cache ARP è gestita dal kernel.
   - Può essere visualizzata utilizzando il comando `arp` in un terminale.

COMANDI  per visualizzare la cache ARP su Linux, Windows e macOS:



**Linux:**
  ```bash
  arp -n
  arp -v 
  ```

**Windows:**
  ```bash
  arp -a
  ```

**macOS:**
  ```bash
  arp -a
  ```

le voci nella cache ARP sono temporanee e possono essere sovrascritte o rimosse nel tempo.
Inoltre, la cache ARP è specifica per ogni dispositivo e non è condivisa tra i dispositivi nella rete.


**VULNS**


Il Protocollo di Risoluzione degli Indirizzi (ARP) è vulnerabile ad alcuni tipi di attacchi, spesso noti come attacchi ARP spoofing o attacchi di avvelenamento ARP. Questi attacchi sfruttano la natura trust-based e non autenticata del protocollo ARP. Alcuni degli attacchi ARP più comuni includono:

**ARP Spoofing (ARP Poisoning):**
   In questo attacco, un attaccante invia pacchetti ARP falsificati alla rete, affermando di possedere l'indirizzo IP di un altro dispositivo (come il gateway predefinito). Questo può portare a un'inversione delle associazioni ARP nella cache degli altri dispositivi, facendo sì che inviino il traffico destinato a quell'indirizzo IP al dispositivo compromesso.

**ARP Cache Poisoning:**
   Simile all'ARP spoofing, l'ARP cache poisoning coinvolge la manipolazione delle informazioni nella cache ARP di un dispositivo. Gli attaccanti inviano pacchetti ARP falsificati per aggiornare la cache ARP di un dispositivo con informazioni errate.

**Man-in-the-Middle (MITM) con ARP:**
   In un attacco MITM, un attaccante può sfruttare il protocollo ARP per intercettare e manipolare il traffico tra due dispositivi sulla rete. Ciò può consentire all'attaccante di monitorare o modificare i dati in transito.

**ARP Request Flooding:**
   Gli attaccanti possono inundare la rete con numerose richieste ARP false, sovraccaricando la cache ARP dei dispositivi e causando rallentamenti o interruzioni del traffico di rete.


CONTROMISURE POSSIBILI :

- **Static ARP Entries:** Configurare voci ARP statiche nelle cache ARP dei dispositivi, in modo che le associazioni siano meno suscettibili a essere sovrascritte.

- **ARP Inspection:** Alcuni switch supportano la funzionalità di ARP inspection, che può rilevare e mitigare attacchi ARP spoofing.

- **VPN e Tunneling:** Utilizzare reti private virtuali (VPN) o tunneling per proteggere il traffico da attacchi MITM sulla rete locale.

- **Monitoraggio del Traffico ARP:** Monitorare attentamente il traffico ARP e rilevare anomalie o modelli sospetti che potrebbero indicare attività fraudolenta.



**ESERCITAZIONE**


Il protocollo ARP non prevede l'autenticazione, quindi l'hacker può facilmente utilizzare questa "funzione" per scoprire tutti i sistemi di una rete. Ciò può essere utile quando si cerca di violare un altro sistema sulla rete locale (LAN) o quando si compromette un singolo utente sulla rete e si vuole passare a un obiettivo più prezioso sulla rete, come un server di database.
Esistono numerosi strumenti che l'hacker può utilizzare per scoprire i sistemi sulla rete. Questi strumenti inviano una richiesta ARP  e i sistemi rispondono con il loro indirizzo IP e MAC. Per esempio, nel nostro sistema Kali, abbiamo netdiscover.
Per visualizzare la schermata di aiuto di netdiscover, basta inserire;

```
sudo netdiscover -h
```


**ALCUNI TOOLS PER MAN-IN-THE-MIDDLE**

> ARP SPOOF ( VEDI TUTORIAL )
> DRIFNET ( VEDI TUTORIAL )



<img width="625" alt="Screenshot 2024-02-11 alle 13 16 42" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/64ff2e01-4db9-4fae-b776-cd15e337757f">



_____________________________________________________________

# Domain Name Service (DNS)


Il Domain Name System o DNS è uno dei protocolli di rete che fanno girare il mondo. Senza di esso, dovremmo ricordare innumerevoli indirizzi IP solo per navigare verso i nostri siti web preferiti. Immaginate di dover ricordare gli indirizzi IPv4 (32 bit) di Facebook, Amazon e Hackers-Arise, solo per visitare ciascuno di questi siti web di importanza critica (il che è peggiorato dagli indirizzi IPv6 a 128 bit).
Il DNS è stato progettato per tradurre un nome di dominio - qualcosa che le persone sono piuttosto brave a ricordare - in un indirizzo IP, il linguaggio del routing di Internet. Il DNS è semplicemente la traduzione di un nome di dominio nei rispettivi indirizzi IP.




**comandi utili**



**`dig` (Domain Information Groper):**
   `dig` è un potente strumento di interrogazione DNS che consente di ottenere informazioni dettagliate sui record DNS. Può essere utilizzato per ottenere informazioni come gli indirizzi IP associati a un nome di dominio, i record MX (Mail Exchange), i record TXT, ecc.

   ```bash
   dig example.com
   ```

**`nslookup` (Name Server Lookup):**
   `nslookup` è un comando diagnostico che consente di eseguire interrogazioni DNS e ottenere informazioni sui server DNS. Tuttavia, questo comando è stato sostituito da `dig` e potrebbe non essere presente in tutte le distribuzioni.

   ```bash
   nslookup example.com
   ```

**`host`:**
   `host` è un comando che fornisce informazioni DNS di base, come l'indirizzo IP associato a un nome di dominio.

   ```bash
   host example.com
   ```

**`hostname`:**
   `hostname` restituisce il nome host associato all'indirizzo IP del sistema locale. Può anche essere utilizzato con l'opzione `-i` per ottenere direttamente l'indirizzo IP.

   ```bash
   hostname
   ```

   ```bash
   hostname -i
   ```

**`whois`:**
   `whois` non è specificamente un comando DNS, ma può essere utilizzato per ottenere informazioni sul proprietario di un dominio e dettagli associati.

   ```bash
   whois example.com
   ```

**`nmcli` (NetworkManager Command-Line Interface):**
   Se stai utilizzando NetworkManager, `nmcli` può essere utilizzato per visualizzare informazioni sulla connessione di rete corrente, inclusi i server DNS.

   ```bash
   nmcli dev show | grep DNS
   ```


I nomi di dominio devono essere registrati presso l'ICANN (Internet Corporation for Assigned Names and Numbers), di solito tramite un intermediario come VeriSign o GoDaddy. I domini di primo livello (TLD) comprendono .com, .edu, .org e molti altri che di solito si vedono alla fine di un nome di dominio completamente qualificato (FQDN).

<img width="549" alt="Screenshot 2024-02-11 alle 13 27 08" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/88be685d-abdf-43c5-afd8-42760de97f14">


Il DNS funziona in modo gerarchico. I domini di primo livello o TLD possono avere più sottodomini.



**Panoramica sul DNS:**

Il Domain Name System (DNS) è un sistema distribuito che consente di associare nomi di dominio a indirizzi IP e viceversa. Funziona come un grande elenco telefonico distribuito su Internet, consentendo agli utenti di utilizzare nomi di dominio più memorizzabili al posto di indirizzi IP numerici per accedere a risorse online.

Il DNS svolge un ruolo cruciale nelle comunicazioni su Internet, poiché molti protocolli, come HTTP, utilizzano nomi di dominio per identificare i server. Il sistema DNS è basato su una struttura gerarchica che consente la distribuzione delle responsabilità tra diversi server DNS.

**Componenti chiave del DNS:**

**Root DNS Server:**
   Il sistema DNS inizia con i server radice, che sono al vertice della gerarchia. Ci sono un piccolo numero di server radice, etichettati con lettere dalla A alla M. Questi server indicano dove trovare i server DNS autoritativi per i domini di primo livello (TLD).

**Server DNS dei Top-Level Domain (TLD):**
   I server TLD gestiscono le richieste per i domini di primo livello (.com, .org, .net, ecc.). Esistono server TLD per ciascuna estensione di dominio, e questi server forniscono informazioni su dove trovare i server DNS autoritativi per i domini di secondo livello.

**Server DNS Autoritativo:**
   Questi server contengono informazioni dettagliate sui nomi di dominio, compresi gli indirizzi IP associati e altre informazioni come record MX (per la posta) e record NS (per i server dei nomi). Ogni dominio ha almeno uno o più server DNS autoritativi.

 **Server DNS Ricorsivo:**
   Questi server gestiscono le richieste DNS degli utenti finali. Quando un utente cerca di accedere a un sito web, il server DNS ricorsivo effettua una serie di richieste ai server radice, ai server TLD e ai server autoritativi per risolvere il nome di dominio in un indirizzo IP.

**Funzionamento del DNS:**

**Richiesta DNS Ricorsiva:**
   Quando un dispositivo cerca di accedere a un sito web tramite un nome di dominio, il server DNS ricorsivo del provider di servizi Internet (ISP) o del servizio locale effettua una richiesta al sistema DNS per risolvere il nome di dominio.

**Risoluzione del Dominio:**
   Il server DNS ricorsivo inizia con una richiesta ai server radice, che indicano il server TLD appropriato. Successivamente, il server TLD indica il server DNS autoritativo per il dominio specifico.

**Cache DNS:**
   I server DNS ricorsivi mantengono una cache locale delle risoluzioni DNS recenti. Questa cache riduce il tempo di risoluzione, in quanto i risultati possono essere recuperati direttamente dalla cache se sono stati risolti di recente.

**Tempo di Vita (TTL):**
   Ogni record DNS contiene un parametro chiamato "Time to Live" (TTL), che specifica per quanto tempo le informazioni devono essere memorizzate nella cache. Dopo il periodo TTL, il record viene rimosso dalla cache e deve essere nuovamente risolto.


**ESERCITAZIONE**

Per monitorare tutti i passaggi relativi alle richieste DNS, utilizziamo comando `dig` (Domain Information Groper) con l'opzione `+trace`. Questa opzione consente di visualizzare la sequenza completa di richieste DNS dalla tua macchina fino al server autoritativo del dominio.


```bash
dig +trace example.com
```

Sostituisci "example.com" con il nome di dominio che desideri analizzare. L'output mostrerà una sequenza di richieste DNS, partendo dai server radice e passando attraverso i server TLD e i server autoritativi fino a raggiungere l'indirizzo IP finale associato al nome di dominio.

L'output sarà dettagliato e mostrerà ciascun passo del processo di risoluzione DNS, inclusi i server coinvolti, i tempi di risposta e gli indirizzi IP associati ai nomi di dominio. Utilizzando `+trace`, si ottiene una visione completa di come avviene la risoluzione DNS per il dominio specificato.



Il sistema di Nome di Dominio (DNS) è composto da quattro componenti principali che lavorano insieme per facilitare la risoluzione dei nomi di dominio in indirizzi IP e viceversa. 

1. **Cache DNS:**
   - **Descrizione:** La cache DNS è una posizione di memorizzazione temporanea utilizzata per conservare le richieste DNS risolte in precedenza. Questa cache contribuisce a migliorare l'efficienza e la velocità delle richieste DNS successive evitando di dover ripetere l'intero processo di risoluzione per i nomi di dominio frequentemente accessati.
   - **Funzione:** Quando un risolutore DNS o un server di nomi riceve una richiesta per un nome di dominio, prima controlla la sua cache locale. Se le informazioni sono presenti (a seguito di una richiesta recente), può rispondere immediatamente senza dover ripetere l'intera procedura di risoluzione.

2. **Risolvitori (Resolvers):**
   - **Descrizione:** I risolutori sono componenti software o hardware che inviano richieste DNS e gestiscono il processo di risoluzione. I risolutori sono spesso parte del sistema operativo o inclusi nei programmi dei browser web.
   - **Funzione:** Quando un'applicazione o un dispositivo richiede la risoluzione di un nome di dominio, il risolutore si occupa di inoltrare la richiesta ai server DNS appropriati e ricevere la risposta.

3. **Server di Nomi (Name Servers):**
   - **Descrizione:** I server di nomi sono server specializzati responsabili della memorizzazione delle informazioni DNS per un dominio specifico. Possono essere divisi in server autoritativi e server ricorsivi.
   - **Funzione:** I server autoritativi detengono le informazioni ufficiali su un dominio, mentre i server ricorsivi aiutano a risolvere le richieste inviate loro, cercando le informazioni attraverso la gerarchia DNS.

4. **Spazio dei Nomi (Name Space):**
   - **Descrizione:** Lo spazio dei nomi è una gerarchia strutturata e organizzata in cui sono assegnati i nomi di dominio. La gerarchia parte dal livello più alto, noto come la radice, e si dirama attraverso i domini di primo livello (TLD), i domini di secondo livello e così via.
   - **Funzione:** Lo spazio dei nomi fornisce una struttura organizzativa per i nomi di dominio e stabilisce le regole per la creazione e l'assegnazione di nuovi domini all'interno della gerarchia. La radice, i TLD e i domini di secondo livello costituiscono parte integrante di questo spazio gerarchico.



<img width="547" alt="Screenshot 2024-02-11 alle 14 27 33" src="https://github.com/MrMagicalSoftware/complete-academy-cybersec/assets/98833112/e670bb61-181f-45c6-b4cd-e897a6c5ea2e">

I record DNS (Domain Name System) contengono informazioni cruciali per la risoluzione dei nomi di dominio in indirizzi IP e svolgono un ruolo essenziale nel funzionamento di Internet. Ci sono diverse tipologie di record DNS, ognuna delle quali svolge una funzione specifica. Ecco alcune delle tipologie di record DNS più comuni:

**Record A (Address Record):**
   - **Descrizione:** Associa un nome di dominio a un indirizzo IPv4.
   - **Esempio:** `example.com IN A 192.168.1.1`

**Record AAAA (IPv6 Address Record):**
   - **Descrizione:** Associa un nome di dominio a un indirizzo IPv6.
   - **Esempio:** `example.com IN AAAA 2001:0db8:85a3:0000:0000:8a2e:0370:7334`

 **Record CNAME (Canonical Name):**
   - **Descrizione:** Crea un alias per un altro nome di dominio (il nome canonico). Spesso utilizzato per puntare un sotto-dominio a un dominio principale.
   - **Esempio:** `www.example.com IN CNAME example.com`

 **Record MX (Mail Exchange):**
   - **Descrizione:** Specifica i server di posta responsabili della ricezione delle email per un dominio.
   - **Esempio:** `example.com IN MX 10 mail.example.com`

 **Record PTR (Pointer Record):**
   - **Descrizione:** Utilizzato per la risoluzione inversa, associa un indirizzo IP a un nome di dominio.
   - **Esempio:** `1.1.168.192.in-addr.arpa IN PTR example.com`

**Record NS (Name Server):**
   - **Descrizione:** Specifica i server di nomi autoritativi per un dominio.
   - **Esempio:** `example.com IN NS ns1.example.com`

**Record SOA (Start of Authority):**
   - **Descrizione:** Fornisce informazioni sulla zona DNS, inclusi i parametri di gestione della zona.
   - **Esempio:** `example.com IN SOA ns1.example.com admin.example.com 2022021001 86400 7200 3600000 86400`

 **Record TXT (Text):**
   - **Descrizione:** Contiene testo libero o informazioni strutturate. Utilizzato per scopi vari, tra cui la verifica di proprietà dei domini e la fornitura di informazioni sul dominio.
   - **Esempio:** `example.com IN TXT "Questo è un record TXT di esempio"`


Il record SOA (Start of Authority) è uno dei record DNS (Domain Name System) fondamentali e svolge un ruolo chiave nella gestione di una zona DNS. Una zona DNS rappresenta una parte gerarchica dello spazio dei nomi del DNS, ed è gestita da un singolo server DNS autoritativo. Il record SOA fornisce informazioni essenziali su questa zona. in dettaglio record SOA:

Il record SOA è essenziale per la corretta gestione delle zone DNS, garantendo la sincronizzazione tra i server DNS primari e secondari e fornendo informazioni critiche sulla configurazione e l'autorità della zona.


**Struttura del Record SOA:**
```
example.com IN SOA ns1.example.com admin.example.com (
                2022021001 ; Numero di serie
                86400      ; Intervallo di riflessione (Refresh)
                7200       ; Ritardo di ritrasmissione (Retry)
                3600000    ; Tempo massimo di scadenza (Expire)
                86400 )    ; Tempo minimo di TTL (Time to Live)
```

**Descrizione dei campi:**

1. **Nome del dominio principale (example.com):**
   - Indica la zona del dominio principale associata a questo record SOA.

2. **Nome del server primario (ns1.example.com):**
   - Specifica il server di nomi primario autoritativo per la zona. Questo è il server che contiene l'autorità finale sulla zona e ha il controllo principale sulla gestione delle informazioni DNS per quella zona.

3. **Indirizzo email dell'amministratore (admin.example.com):**
   - Indica l'indirizzo email dell'amministratore responsabile della zona. Nella rappresentazione del record SOA, l'indirizzo email è invertito e il punto è sostituito da un punto e virgola.

4. **Numero di serie (2022021001):**
   - Rappresenta il numero di versione della zona. Questo numero dovrebbe essere incrementato ogni volta che vengono apportate modifiche alla zona. Aiuta a garantire che i server DNS in giro per il mondo siano consapevoli delle nuove informazioni.

5. **Intervallo di riflessione (Refresh):**
   - Indica il periodo di tempo in secondi dopo il quale un server DNS secondario dovrebbe verificare se il record SOA è cambiato. In caso di modifiche, il server secondario inizierà il processo di trasferimento di zona.

6. **Ritardo di ritrasmissione (Retry):**
   - Specifica il tempo in secondi che un server secondario dovrebbe attendere prima di tentare di riconnettersi al server primario nel caso di un fallimento di trasferimento di zona.

7. **Tempo massimo di scadenza (Expire):**
   - Indica il periodo di tempo massimo in secondi durante il quale un server secondario può utilizzare le informazioni DNS se non riesce a comunicare con il server primario. Dopo questo periodo, il server secondario non risponderà più alle query per quella zona.

8. **Tempo minimo di TTL (Time to Live):**
   - Specifica il valore minimo di TTL per tutti gli altri record nella zona. Il TTL è il periodo di tempo per cui un record può essere mantenuto nella cache di un client DNS prima che debba essere nuovamente verificato.




