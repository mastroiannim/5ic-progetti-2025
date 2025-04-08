**Domanda articolata:**

Immagina di dover progettare una rete aziendale per una piccola impresa che ha bisogno di connettere i propri uffici distribuiti in diverse sedi geografiche. L'azienda richiede che la rete sia sicura, affidabile e in grado di supportare servizi critici come videoconferenze, trasferimento di file sensibili e accesso remoto ai sistemi interni.

1. **Problematica:** Quali sono le principali sfide legate alla progettazione di una rete aziendale basata su un'architettura stratificata (es. modello OSI o TCP/IP)? In particolare, come si possono affrontare problemi legati alla sicurezza (es. protezione dei dati), alla gestione del traffico (es. priorità per servizi critici) e alla interoperabilità tra dispositivi di fornitori diversi?

2. **Soluzione:** Descrivi come struttureresti la rete utilizzando il modello a strati (OSI o TCP/IP). Specifica:  
   - Come organizzeresti i vari livelli (es. fisico, data link, rete, trasporto, applicazione) per soddisfare i requisiti dell'azienda.  
   - Quali tecnologie adotteresti per garantire sicurezza, affidabilità e priorità del traffico.  
   - Un esempio pratico di come implementeresti un servizio critico, come le videoconferenze, sfruttando i livelli del modello OSI.

3. **Tecnologie:** Quali tecnologie e protocolli utilizzeresti per implementare la rete completa e perché? Considera aspetti come dispositivi di rete (router, switch, firewall), protocolli di comunicazione (es. IPsec, VLAN, QoS) e strumenti di monitoraggio. Inoltre, discuti come gestiresti situazioni di emergenza, come un'interruzione della connettività o un attacco informatico.

---

**Spiegazione della domanda:**

Questa domanda è stata formulata per far emergere diverse competenze acquisite durante il corso sulle architetture di rete:

1. **Problematica:** Si richiede allo studente di identificare i problemi tipici delle reti aziendali, come la sicurezza, la gestione del traffico e l'interoperabilità tra dispositivi. Questo permette di valutare la capacità critica di individuare le sfide principali e proporre soluzioni basate sui livelli del modello OSI o TCP/IP.

2. **Soluzione:** Lo studente deve dimostrare di comprendere come organizzare i vari livelli dell'architettura di rete per soddisfare i requisiti aziendali. Deve descrivere come ogni livello contribuisce alla sicurezza, all'affidabilità e alla priorità del traffico, fornendo un esempio pratico di implementazione di un servizio critico.

3. **Tecnologie:** La parte finale della domanda richiede allo studente di fare scelte tecnologiche motivate, dimostrando di conoscere gli strumenti moderni utilizzati nel settore. Ad esempio, potrebbe citare tecnologie come VLAN per segmentare il traffico, QoS per priorizzare i servizi critici e IPsec per proteggere i dati. Infine, deve mostrare di sapere come gestire situazioni di emergenza.

---

**Esempio di risposta attesa:**

1. **Problematica:**  
   - Problemi:  
     - **Sicurezza:** Proteggere i dati sensibili da intercettazioni e attacchi informatici.  
     - **Gestione del traffico:** Garantire che servizi critici come videoconferenze abbiano priorità sul traffico meno importante.  
     - **Interoperabilità:** Assicurarsi che dispositivi di fornitori diversi possano comunicare senza problemi.  
   - Soluzioni:  
     - Utilizzerei protocolli di cifratura (es. IPsec, SSL/TLS) per proteggere i dati.  
     - Implementerei QoS (Quality of Service) per prioritizzare il traffico critico.  
     - Standardizzerei i protocolli di comunicazione (es. IPv4/IPv6) per garantire interoperabilità.  

2. **Soluzione:**  
   - **Livello fisico:** Utilizzerei cavi in fibra ottica per connessioni veloci e affidabili tra le sedi.  
   - **Livello data link:** Configurerei VLAN per segmentare il traffico e ridurre il rischio di collisioni o attacchi interni.  
   - **Livello rete:** Userei router con supporto per IPv6 e protocolli di routing dinamico (es. OSPF) per gestire il traffico tra le sedi.  
   - **Livello trasporto:** Implementerei il protocollo TCP per garantire la consegna affidabile dei pacchetti e configurerei QoS per prioritizzare servizi critici come le videoconferenze.  
   - **Livello applicazione:** Utilizzerei protocolli sicuri come HTTPS e SIP (per le videoconferenze) e integrerei un firewall per filtrare il traffico malevolo.  
   - **Esempio pratico (videoconferenze):**  
     - Al livello applicazione, utilizzerei il protocollo SIP per stabilire la sessione di videoconferenza.  
     - Al livello trasporto, configurerei QoS per garantire banda sufficiente e bassa latenza.  
     - Al livello rete, userei IPsec per cifrare il traffico tra le sedi.  

3. **Tecnologie:**  
   - **Dispositivi di rete:** Router Cisco o Juniper per il routing dinamico, switch gestiti per configurare VLAN e firewall per proteggere la rete.  
   - **Protocolli:**  
     - IPsec per la cifratura del traffico.  
     - VLAN per segmentare il traffico.  
     - QoS per prioritizzare i servizi critici.  
   - **Monitoraggio:** Utilizzerei strumenti come Nagios o PRTG per monitorare lo stato della rete e rilevare anomalie in tempo reale.  
   - **Gestione emergenze:** Implementerei un sistema di backup della connettività (es. linea DSL come failover) e configurerei un IDS/IPS (Intrusion Detection/Prevention System) per rilevare e mitigare attacchi informatici.  

**Risultato finale:** La domanda permette di valutare in modo completo le competenze teoriche e pratiche dello studente, evidenziando sia la comprensione dei principi delle architetture di rete sia la capacità di applicarli in un contesto reale.
