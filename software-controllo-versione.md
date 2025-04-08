**Domanda articolata:**

Immagina di lavorare in un team di sviluppo che sta collaborando alla creazione di un'applicazione web. Il progetto è complesso e coinvolge più sviluppatori che lavorano contemporaneamente su diverse funzionalità. Durante lo sviluppo, si verificano situazioni in cui due sviluppatori modificano lo stesso file, causando conflitti, oppure si ha la necessità di tornare a una versione precedente del codice per correggere un errore introdotto recentemente.

1. **Problematica:** Quali sono i principali problemi che si presentano quando un team di sviluppo lavora su un progetto software senza utilizzare strumenti di controllo versione? Come si possono gestire situazioni come i conflitti tra modifiche o il ripristino di versioni precedenti del codice?

2. **Soluzione:** Descrivi come utilizzeresti **Git** per gestire il controllo versione del progetto. Specifica:  
   - Quali comandi Git useresti per risolvere un conflitto tra due sviluppatori che hanno modificato lo stesso file.  
   - Come organizzeresti il workflow del team (es. branch, commit, merge) per garantire una collaborazione efficace e ridurre i conflitti.  
   - Un esempio pratico di come ripristineresti una versione precedente del codice in caso di errore critico.

3. **Tecnologie:** Quali piattaforme e strumenti utilizzeresti per ospitare il repository Git e perché? Considera aspetti come la collaborazione, la sicurezza e l'integrazione con altri strumenti di sviluppo. Inoltre, discuti come monitoreresti lo stato del repository e gestiresti eventuali errori durante il processo di integrazione continua.

---

**Spiegazione della domanda:**

Questa domanda è stata formulata per far emergere diverse competenze acquisite durante il corso sull'introduzione a Git e ai software di controllo versione:

1. **Problematica:** Si richiede allo studente di identificare i problemi legati alla mancanza di un sistema di controllo versione, come la sovrapposizione delle modifiche, la perdita di versioni precedenti del codice e la difficoltà di collaborazione in team. Questo permette di valutare la capacità critica di individuare le sfide tipiche nello sviluppo collaborativo.

2. **Soluzione:** Lo studente deve dimostrare di comprendere come utilizzare Git per risolvere problemi comuni, come conflitti tra modifiche e ripristino di versioni precedenti. Deve descrivere un workflow organizzato (es. uso di branch, commit frequenti, pull request) e fornire esempi pratici di comandi Git. Questo evidenzia la capacità di applicare i concetti teorici in un contesto reale.

3. **Tecnologie:** La parte finale della domanda richiede allo studente di fare scelte tecnologiche motivate, dimostrando di conoscere le piattaforme moderne utilizzate per ospitare repository Git, come GitHub, GitLab o Bitbucket. Inoltre, deve mostrare di sapere come integrare Git con strumenti di automazione e monitoraggio, come CI/CD pipelines.

---

**Esempio di risposta attesa:**

1. **Problematica:**  
   - Problemi: Senza un sistema di controllo versione, è difficile tenere traccia delle modifiche, collaborare in modo efficace e ripristinare versioni precedenti del codice. Situazioni come conflitti tra modifiche o errori introdotti accidentalmente possono rallentare il lavoro del team.  
   - Soluzioni: Utilizzando Git, possiamo gestire le modifiche in modo strutturato, risolvere conflitti in modo efficiente e mantenere uno storico delle versioni per ripristinare lo stato precedente del codice in caso di necessità.

2. **Soluzione:**  
   - **Risoluzione conflitti:** Se due sviluppatori modificano lo stesso file, utilizzerei i seguenti comandi:  
     1. `git pull` per scaricare le modifiche remote.  
     2. Risolvere manualmente i conflitti nel file interessato.  
     3. `git add <file>` per segnalare che il conflitto è risolto.  
     4. `git commit` per completare il merge.  
   - **Workflow:**  
     - Ogni sviluppatore lavora su un branch separato per ogni funzionalità (`git checkout -b feature/nome-feature`).  
     - Una volta completata la funzionalità, il branch viene unito al branch principale tramite pull request (`git merge` o `git rebase`).  
     - Commit frequenti con messaggi chiari per documentare le modifiche.  
   - **Ripristino versione:** Per tornare a una versione precedente del codice, userei:  
     1. `git log` per identificare il commit desiderato.  
     2. `git checkout <commit-id>` per visualizzare lo stato del codice in quel commit.  
     3. Se necessario, creare un nuovo branch da quel commit (`git checkout -b hotfix-branch`) per apportare correzioni.  

3. **Tecnologie:**  
   - Piattaforma: Utilizzerei **GitHub** per ospitare il repository, poiché offre strumenti avanzati per la collaborazione, come pull request, code review e issue tracking.  
   - Sicurezza: Configurerei autenticazione a due fattori (2FA) e limiterei i permessi di accesso al repository.  
   - Integrazione continua: Utilizzerei GitHub Actions per automatizzare test e deployment. Ad esempio, configurerei una pipeline che esegue test automatici ogni volta che viene effettuato un push sul repository.  
   - Monitoraggio: Userei strumenti come **SonarQube** per analizzare la qualità del codice e rilevare vulnerabilità.

**Risultato finale:** La domanda permette di valutare in modo completo le competenze teoriche e pratiche dello studente, evidenziando sia la comprensione dei principi di Git e del controllo versione sia la capacità di applicarli in un contesto di sviluppo collaborativo.
