**Domanda articolata:**

Immagina di dover progettare un sistema basato su **architettura REST** per una piattaforma di gestione di eventi culturali. La piattaforma deve permettere agli utenti di visualizzare gli eventi disponibili, prenotarsi a un evento, visualizzare le proprie prenotazioni e cancellarle. Inoltre, il sistema deve essere facilmente scalabile e interoperabile con altre applicazioni.

1. **Problematica:** Quali sono i principali vantaggi e limiti dell'architettura REST in questo contesto? Come si possono affrontare eventuali problemi legati alla scalabilità, all'efficienza delle comunicazioni e all'interoperabilità con altri sistemi?

2. **Soluzione:** Descrivi come struttureresti l'API RESTful per soddisfare i requisiti del sistema, specificando:  
   - I principi fondamentali dell'architettura REST che hai applicato (es. statelessness, uniform interface, resource-based design).  
   - Gli endpoint che definiresti, i metodi HTTP appropriati (GET, POST, PUT, DELETE) e i percorsi delle risorse.  
   - Un esempio di risposta JSON per uno degli endpoint.  

3. **Tecnologie:** Quali tecnologie utilizzeresti per implementare questa API e perché? Considera sia il lato server (linguaggi di programmazione, framework, database) sia il lato client (strumenti per consumare l'API). Inoltre, discuti come garantiresti prestazioni ottimali e scalabilità del sistema, ad esempio tramite caching o load balancing.

---

**Spiegazione della domanda:**

Questa domanda è stata formulata per far emergere diverse competenze acquisite durante il corso sull'architettura REST:

1. **Problematica:** Si richiede allo studente di analizzare i vantaggi e i limiti dell'architettura REST in un contesto reale, evidenziando aspetti come la scalabilità, l'efficienza delle comunicazioni e l'interoperabilità. Questo permette di valutare la capacità critica di individuare i punti di forza e di debolezza di un sistema basato su REST.

2. **Soluzione:** Lo studente deve dimostrare di comprendere i principi fondamentali dell'architettura REST e di saperli applicare nella progettazione di un'API. Deve descrivere come strutturare gli endpoint in modo logico e coerente, scegliendo i metodi HTTP appropriati e fornendo un esempio di risposta JSON. Questo evidenzia la capacità di tradurre i principi teorici in una soluzione pratica.

3. **Tecnologie:** La parte finale della domanda richiede allo studente di fare scelte tecnologiche motivate, dimostrando di conoscere gli strumenti moderni utilizzati nel settore. Ad esempio, potrebbe citare linguaggi come Python (con Flask o FastAPI), Node.js (con Express), o Java (con Spring Boot) per il backend, e database come MySQL o MongoDB per la persistenza dei dati. Per il lato client, potrebbe menzionare strumenti come Axios o Fetch API per consumare l'API. Infine, deve mostrare di sapere come ottimizzare le prestazioni e garantire la scalabilità.

---

**Esempio di risposta attesa:**

1. **Problematica:**  
   - Vantaggi: L'architettura REST è ideale per sistemi distribuiti grazie alla sua natura stateless, che semplifica la scalabilità e l'indipendenza tra client e server. Inoltre, l'uso di standard come HTTP e JSON favorisce l'interoperabilità.  
   - Limiti: Uno svantaggio è la possibile inefficienza delle comunicazioni se non si adottano strategie di caching. Inoltre, la mancanza di uno stato condiviso può complicare alcune operazioni che richiedono sessioni persistenti.  
   - Soluzioni: Per affrontare questi limiti, implementerei caching tramite HTTP headers (es. `Cache-Control`) e userei un load balancer per distribuire il carico su più server.

2. **Soluzione:**  
   - Principi applicati:  
     - **Statelessness:** Ogni richiesta contiene tutte le informazioni necessarie per essere elaborata dal server.  
     - **Uniform Interface:** Uso di URI ben definiti per rappresentare le risorse e metodi HTTP standard per interagire con esse.  
     - **Resource-based design:** Le risorse principali sono "eventi" e "prenotazioni".  
   - Endpoint:  
     - `GET /events` → Visualizza tutti gli eventi disponibili.  
     - `POST /bookings` → Crea una nuova prenotazione.  
     - `GET /bookings/{user_id}` → Visualizza le prenotazioni di un utente.  
     - `DELETE /bookings/{booking_id}` → Cancella una prenotazione.  
   - Esempio di risposta JSON per `GET /events`:  
     ```json
     [
       {
         "id": 1,
         "name": "Concerto di Natale",
         "date": "2023-12-24",
         "location": "Teatro Comunale"
       },
       {
         "id": 2,
         "name": "Mostra d'Arte Contemporanea",
         "date": "2023-11-15",
         "location": "Galleria Moderna"
       }
     ]
     ```

3. **Tecnologie:**  
   - Backend: Utilizzerei Node.js con Express per la sua leggerezza e facilità di integrazione con database NoSQL come MongoDB.  
   - Database: MongoDB per la flessibilità dello schema e la velocità nelle query.  
   - Client: Uso Axios per consumare l'API in un'applicazione frontend React.  
   - Ottimizzazione: Implementerei caching con Redis per ridurre il carico sul database e userei un load balancer (es. Nginx) per distribuire le richieste su più server.  
   - Scalabilità: Utilizzerei containerizzazione con Docker e orchestrazione con Kubernetes per gestire la scalabilità automatica del sistema.

**Risultato finale:** La domanda permette di valutare in modo completo le competenze teoriche e pratiche dello studente, evidenziando sia la comprensione dei principi dell'architettura REST sia la capacità di applicarli in un contesto reale.
