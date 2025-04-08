**Domanda articolata:**

Immagina di dover progettare un sistema distribuito per un'applicazione di e-commerce che gestisce milioni di utenti simultaneamente. L'applicazione deve garantire un accesso rapido e affidabile ai dati (es. catalogo prodotti, carrelli degli utenti), scalabilità per gestire picchi di traffico durante le promozioni e tolleranza ai guasti per evitare interruzioni del servizio in caso di malfunzionamenti.

1. **Problematica:** Quali sono i principali problemi legati alla progettazione di un sistema distribuito come quello descritto? In particolare, come si possono affrontare le sfide legate alla trasparenza dell'accesso (nascondere la distribuzione agli utenti), alla scalabilità orizzontale e alla tolleranza ai guasti?

2. **Soluzione:** Descrivi come struttureresti il sistema distribuito per soddisfare i requisiti sopra elencati. Specifica:  
   - Come garantiresti la trasparenza dell'accesso, in modo che gli utenti non si accorgano della distribuzione dei dati tra più server.  
   - Quali strategie adotteresti per garantire scalabilità orizzontale (aggiunta di nuovi nodi) e gestire picchi di traffico.  
   - Come implementeresti meccanismi di tolleranza ai guasti per evitare interruzioni del servizio in caso di malfunzionamenti hardware o software.  

3. **Tecnologie:** Quali tecnologie utilizzeresti per implementare questo sistema distribuito e perché? Considera aspetti come database distribuiti, load balancing, caching e containerizzazione. Inoltre, discuti come monitoreresti lo stato del sistema e gestiresti eventuali emergenze.

---

**Spiegazione della domanda:**

Questa domanda è stata formulata per far emergere diverse competenze acquisite durante il corso sui sistemi distribuiti e le forme di trasparenza:

1. **Problematica:** Si richiede allo studente di identificare i problemi tipici dei sistemi distribuiti, come la complessità di nascondere la distribuzione agli utenti (trasparenza dell'accesso), la necessità di scalare dinamicamente per gestire carichi elevati e la garanzia di continuità del servizio in caso di guasti. Questo permette di valutare la capacità critica di individuare le sfide principali.

2. **Soluzione:** Lo studente deve dimostrare di comprendere come affrontare queste sfide utilizzando strategie specifiche, come l'uso di database distribuiti, meccanismi di load balancing e tecniche di replica per la tolleranza ai guasti. Deve anche descrivere un flusso completo che evidenzi come queste soluzioni si integrano nel sistema.

3. **Tecnologie:** La parte finale della domanda richiede allo studente di fare scelte tecnologiche motivate, dimostrando di conoscere gli strumenti moderni utilizzati nel settore. Ad esempio, potrebbe citare tecnologie come Kubernetes per la containerizzazione, Redis per il caching, MongoDB o Cassandra per database distribuiti, e strumenti di monitoraggio come Prometheus o Grafana.

---

**Esempio di risposta attesa:**

1. **Problematica:**  
   - Problemi:  
     - **Trasparenza dell'accesso:** Gli utenti devono accedere ai dati senza percepire che questi sono distribuiti su più server.  
     - **Scalabilità:** Durante eventi promozionali, il sistema deve gestire un numero elevato di richieste senza rallentamenti.  
     - **Tolleranza ai guasti:** Il sistema deve continuare a funzionare anche in caso di malfunzionamenti hardware o software.  
   - Soluzioni:  
     - Implementerei un sistema basato su microservizi con database distribuiti per garantire trasparenza e scalabilità.  
     - Userei meccanismi di replica e failover per garantire tolleranza ai guasti.  

2. **Soluzione:**  
   - **Trasparenza dell'accesso:** Utilizzerei un API Gateway per nascondere la distribuzione dei servizi agli utenti. L'API Gateway instraderebbe le richieste verso i microservizi appropriati, semplificando l'interfaccia utente.  
   - **Scalabilità orizzontale:** Implementerei un sistema di load balancing (es. Nginx o AWS Elastic Load Balancer) per distribuire il carico tra più nodi. Utilizzerei containerizzazione con Docker e orchestrazione con Kubernetes per aggiungere o rimuovere nodi dinamicamente.  
   - **Tolleranza ai guasti:** Adotterei una strategia di replica dei dati su più nodi (es. usando un database distribuito come MongoDB o Cassandra). In caso di guasto di un nodo, il sistema reindirizzerebbe automaticamente le richieste verso un nodo secondario.  

3. **Tecnologie:**  
   - **Database distribuito:** MongoDB o Cassandra per garantire scalabilità e tolleranza ai guasti tramite sharding e replica.  
   - **Load balancing:** Nginx o AWS Elastic Load Balancer per distribuire il carico tra i nodi.  
   - **Caching:** Redis per memorizzare i dati frequentemente richiesti (es. catalogo prodotti) e ridurre il carico sui database.  
   - **Containerizzazione e orchestrazione:** Docker per creare container isolati e Kubernetes per gestire la scalabilità e la disponibilità del sistema.  
   - **Monitoraggio:** Utilizzerei Prometheus per raccogliere metriche sullo stato del sistema e Grafana per visualizzarle in dashboard in tempo reale. Configurerei avvisi automatici per notificare eventuali anomalie.  

**Risultato finale:** La domanda permette di valutare in modo completo le competenze teoriche e pratiche dello studente, evidenziando sia la comprensione dei principi dei sistemi distribuiti sia la capacità di applicarli in un contesto reale.
