# Whats-in-Your_Fridge

**Elevator pitch**

**INTRODUZIONE:**
what's in your fridge è l’applicazione di cui non sapevi di aver bisogno per poter aggiungere creatività e sostenibilità nella routine di preparazione di pranzi cene e spuntini.

**PROBLEMA:**
Quante volte ci siamo trovati nella situazione di avere poco tempo e pochi alimenti in frigo per poter prepararsi un pranzo dignitoso ma senza avere la minima idea di cosa poter cucinare o ancora peggio di trovarsi nella situazione di dover buttare del cibo scaduto per essersi scordati di averlo in frigo e per non essere riusciti a trovare una ricetta che possa averlo come ingrediente.

**SOLUZIONE:**
La soluzione è proprio utilizzare WYF che ti permetterà di rinnovare senza sforzo in maniera creativa il tuo modo di cucinare con ciò che hai a disposizione in frigo e in termini di tempo, ma non solo, perché ti aiuterà ad evitare sprechi alimentari inutili suggerendoti le ricette con gli ingredienti in scadenza e a realizzare una lista della spesa intelligente.

**BUSINESS PLAN:**
la fonte di guadagno dell’applicazione si basa su un base di sviluppo freemium, con funzionalità gratis e a pagamento per un'esperienza qualitativa migliore 

**MARKET SIZE:**
Il mercato della gastronomia è a livello mondiale e sempre più in sviluppo specialmente per evitare sprechi alimentari, quest’app potrebbe contribuire esattamente ad evitare questo tipo di sprechi facendo risparmiare soldi alle famiglie e ai singoli permettendo comunque di realizzare pasti creativi e innovativi anche con quel poco che si ha.

**TEAM:**
Ovviamente da ideatore dell’app avrei la quota maggiore dell’azienda, ma per i primi investitori andrei a cedere circa un 10/15% della quota in base al capitale che l'investitore vorrebbe investire,andando pian piano a scalare per i futuri investitori.


**Guida Installazione**
1. **Abilitare virtualizzazione nel BIOS**

-Questo è necessario su Windows prima di installare Docker

2. **Scaricare e installare Docker e Docker-compose**

-Su Windows/Mac: Scaricare e installare Docker Desktop

-Su Linux: Seguire le istruzioni specifiche per la propria distribuzione

3. **Ottenere il progetto**

-scaricare il file docker-compose.yml

5. **Avviare i container**

docker-compose up -d

6. **Accedere all'applicazione**

Aprire il browser e visitare http://localhost




### Descrizione  
**What's in Your Fridge** è un'app innovativa che aiuta gli appassionati di cucina a trovare ricette e idee originali per utilizzare al meglio i pochi ingredienti disponibili nel proprio frigo o dispensa. Permette agli utenti di condividere e consigliare le proprie creazioni culinarie con amici e familiari, favorendo una cucina creativa e sostenibile.  

### Tag Line  
Crea piatti straordinari con ciò che hai a disposizione!  

### Target  
- Appassionati di cucina  
- Persone con poco tempo per fare la spesa  
- Chi vuole ridurre gli sprechi alimentari  

### Problema  
Quante volte ci siamo trovati nella situazione di avere poco tempo e pochi alimenti in frigo per poter preparare un pranzo dignitoso ma senza avere la minima idea di cosa poter cucinare o ancora peggio di trovarsi nella situazione di dover buttare del cibo scaduto per essersi scordati di averlo in frigo e per non essere riusciti a trovare una ricetta che possa averlo come ingrediente.
Whats in Your Fridge risolve questa sfida offrendo ricette basate su ciò che è già presente in casa, evitando sprechi alimentari.  

### Competitor  
- Giallo Zafferano  
- Svuotafrigo  
- Supercook  
- Pimp My Chef  
- AI Chef  
- Cookpad  

### Tecnologie  
- **Frontend**: Vue.js  
- **Backend**: Javascript, Express.js, Cors  
- **Database**: SQLite  
- **API**: RESTful API per gestione ricette, notifiche e utenti  

---

### Requisiti Iniziali  

#### 1. **Creazione Utente**  
- Registrazione tramite email con i seguenti dati:  
  - Username  
  - Nome, cognome  
  - Anno di nascita  
  - Piatto preferito  
  - Password  
- Accesso tramite username e password.  

#### 2. **Caricamento Ricette**  
- Inserimento dettagli della ricetta:  
  - Titolo  
  - Immagine del piatto finito  
  - Difficoltà (facile, media, difficile)  
  - Tipo (antipasto, primo, secondo, dessert, spuntino)  
  - Breve descrizione  
  - Ingredienti essenziali e aggiuntivi  
  - Istruzioni
  - Tempo

#### 3. **Gestione Ingredienti**  
3.1. **Inserimento Manuale degli Ingredienti Disponibili**  
- L’utente può aggiungere, modificare o rimuovere singoli ingredienti o gruppi.  

3.2. **Ricerca Ricette Basata su Ingredienti**  
- Ricette suggerite in base agli ingredienti disponibili, con:  
  - Compatibilità degli ingredienti  
  - Ricette con pochi ingredienti mancanti.  
- Filtri per:  
  - Livello di difficoltà  
  - Tempo di preparazione  

#### 4. **Funzionalità di Condivisione**  
- Condivisione ricette via app con amici.  

#### 5. **Creazione e Modifica Ricette**  
- Possibilità di creare nuove ricette personalizzate con:  
  - Dettagli degli ingredienti  
  - Procedura di preparazione  
  - Tempo di cottura  
  - Foto del piatto  

#### 6. **Lista della Spesa**    
- Funzione di per segnare gli ingredienti acquistati e con la rispettiva scadenza.
   

---

### Funzionalità Secondarie  

#### 1. Notifiche Push  
- Ricette suggerite in base agli ingredienti disponibili.  
- Avvisi per ingredienti in scadenza.  

#### 2. Funzione "Scadenza degli Ingredienti"  
- Avviso su ingredienti in scadenza con suggerimenti di ricette per evitarne lo spreco.  

#### 3. Salvataggio Ricette Preferite  
- Creazione di una lista personalizzata di ricette salvate.  

#### 4. Valutazioni e Commenti  
- Sistema di valutazione con stelle e recensioni per ogni ricetta.  

---

### Requisiti Non Funzionali  

#### 2. Interfaccia  
- Design responsive e ottimizzato per dispositivi mobili.  

#### 4. Scalabilità  
- Sistema scalabile per gestire utenti e ricette crescenti.  

#### 5. Usabilità  
- Navigazione intuitiva per utenti di ogni livello.  


![Diagramma image](diagramma.jpg)
![Backlog](pb.pdf)
