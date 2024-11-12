# Introduzione a GitHub

GitHub offre strumenti come **Milestone** e **Issues** per gestire i progetti in modo più organizzato, specialmente per i team di sviluppo.

## 1. Milestone

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

## 2. Issues e Task Assignment

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
