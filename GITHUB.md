# Introduzione a GitHub

GitHub offre strumenti come **Milestone** e **Issues** per gestire i progetti in modo più organizzato, specialmente per i team di sviluppo.

## Creare un account su GitHub

Se non hai ancora un account su GitHub, segui questi passaggi:

1. Vai al sito [https://github.com](https://github.com).
2. Clicca su "Sign Up" in alto a destra.
3. Completa la registrazione inserendo un username, una password e un indirizzo email.
4. Segui le istruzioni per confermare il tuo account.

## Creare una nuova Repository

1. Una volta loggato, nella parte superiore della pagina, clicca sul pulsante verde **"New"** o vai direttamente alla pagina [https://github.com/new](https://github.com/new).
2. Nella pagina di creazione della repository, compila i seguenti campi:

   - **Repository Name**: Scegli un nome per la tua repository (ad esempio, `mio-progetto` o `my-project`).
   - **Description (opzionale)**: Aggiungi una breve descrizione del progetto (ad esempio, "Progetto per la creazione di un applicativo...").
   - **Public/Private**: Scegli se la repository sarà pubblica (chiunque può vederla) o privata (solo tu e i collaboratori possono vederla).
   - **Initialize this repository with a README**: Spunta questa opzione per creare automaticamente un file `README.md`, che è utile per descrivere il progetto.
   - **Add .gitignore**: Se desideri aggiungere automaticamente un file `.gitignore`. Se utilizzi macOS è consigliato inserire nel `.gitignore` al primo rigo `.DStore`.
   - **Choose a license**: Se desideri, puoi aggiungere una licenza al tuo progetto. GitHub offre diverse opzioni di licenza.

3. Una volta compilati tutti i campi, clicca su **Create repository**.

Visita [GIT](./GIT.md) per i comandi base per iniziare ad usare git e segui i comandi base dopo la creazione del repository su GitHub.

## Aggiungere un Repository Remoto

Dopo aver creato la repository su GitHub, puoi iniziare a caricare il tuo codice. Se hai già un progetto locale, puoi connetterlo a questa repository remota con i seguenti comandi Git:

1. Apri il terminale sul tuo computer.
2. Naviga nella directory del tuo progetto locale:

   ```bash
   cd /percorso/del/tuo/progetto
   ```

## Milestone

Una milestone rappresenta un obiettivo o una fase importante di un progetto. È utile per organizzare e raggruppare le issues e le pull request (PR) in base a uno scopo specifico, come una nuova versione del software, una funzionalità o una scadenza.

### Creare una Milestone

Per creare una Milestone:

1. Vai alla sezione **Issues** del repository.
2. Clicca su **Milestones** che si trova in alto a destra.
3. Seleziona **New milestone**.
4. Dai un nome alla milestone nome_release_versione.
5. Aggiungi descrizione per spiegare l’obiettivo della milestone e in basso aggiungi una data di scadenza.
6. Clicca su **Create milestone**.

### Utilizzo della Milestone

Una volta creata, puoi assegnare issues e pull request alla milestone specifica. In questo modo, avrai un gruppo di task legati a quell’obiettivo, rendendo più semplice tracciare il progresso del progetto verso quella milestone. Ogni milestone fornisce una panoramica del progresso, con una barra di completamento che indica quante issues sono completate rispetto a quelle aperte.

## Issues e Task Assignment

Le **Issues** rappresentano le singole task o problemi di un progetto. Possono includere bug, funzionalità da implementare o altri lavori da fare.

### Creare una Issue

1. Vai alla sezione **Issues** del repository.
2. Clicca su **New issue**.
3. Dai un titolo e una descrizione alla issue, dettagliando cosa va fatto o qual è il problema.
4. Aggiungi eventuali etichette (**labels**) per specificare il tipo di issue, come _bug_, _enhancement_ o _documentation_.
5. Assegna la issue a una milestone, se pertinente.
6. Clicca su **Submit new issue**.

### Assegnare Task (Issues) a Collaboratori

1. All'interno della issue, sulla destra trovi la sezione **Assignees**.
2. Clicca su **Assignees** e seleziona uno o più collaboratori (che devono avere accesso al repository) a cui vuoi assegnare la issue.
3. Se necessario, puoi anche assegnare la stessa issue a più persone, per lavori in team o in caso di task complesse.

### Checklist nelle Issue

Se una issue richiede una serie di passaggi specifici, GitHub permette di creare una checklist utilizzando una lista di task direttamente nella descrizione della issue. Ecco come fare:

```markdown
- [ ] Task 1
- [ ] Task 2
- [ ] Task 3
```
