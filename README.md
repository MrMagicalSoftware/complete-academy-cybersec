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

















