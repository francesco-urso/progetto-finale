1) # Introduzione a GIT

- GIT è un sistema di controllo di versione distribuito
- Permette di gestire e tenere traccia delle modifiche apportate al codice sorgente.

2) ## Storia di GIT

1. **Creazione**: Git è stato creato nel 2005 da Linus Torvalds.
2. **Motivazione**: Linus cercava un sistema di controllo per sostituire "BitKeeper", utilizzato per gestire il kernel Linux.
3. **Sviluppo**: Dopo aver valutato diverse opzioni, Linus decise di creare un nuovo sistema di controllo da zero, chiamato "GIT".
4. **Nome**: Il nome "GIT" fu scelto come abbreviazione di "Global Information Tracker".
5. **Primo rilascio**: Il primo rilascio di GIT avvenne nel 2005.
6. **Popolarità**:GIT è diventato uno degli strumenti più popolari per la gestione del codice sorgente.

3) ## Concetto di repository

La repository di GIT è un luogo dove si memorizzano tutte le versioni del codice sorgente di un progetto. Essa ha le seguenti caratteristiche:

1. **Centralizzato**:  
   Una repository di Git è un luogo centrale dove si memorizzano tutte le versioni del codice sorgente.
   
2. **Versionato**:  
   Una repository contiene tutte le versioni del codice sorgente, quindi è possibile ripristinare una versione precedente se necessario.
   
3. **Distribuito**:  
   Una repository di Git può essere distribuito su più computer, permettendo a più persone di lavorare sullo stesso progetto contemporaneamente.
   
4. **Ramificato**:  
   Una repository di Git consente di creare rami (branch) per lavorare su diverse versioni del codice sorgente contemporaneamente.

4) ## Comandi base di GIT

1. **`git init`**:  
   Crea un nuovo repository di Git nel proprio computer.
   
2. **`git add`**:  
   Aggiunge i file modificati al repository di Git, per includerli in un nuovo commit.
   
3. **`git commit`**:  
   Crea un nuovo commit che rappresenta una versione del codice sorgente.
   
4. **`git status`**:  
   Visualizza lo stato attuale del repository, mostrando quali file sono stati modificati, aggiunti o commitati.
   
5. **`git log`**:  
   Visualizza la cronologia dei commit, mostrando autore, data e messaggio di ogni commit.
   
6. **`git branch`**:  
   Crea un nuovo branch, cioè una versione separata del codice sorgente.
   
7. **`git checkout`**:  
   Permette di passare a un altro branch, per lavorare su una versione diversa del codice sorgente.
   
8. **`git merge`**:  
   Unisce le modifiche apportate in diversi branch, creando una versione unificata del codice sorgente.
   
9. **`git pull`**:  
   Scarica le modifiche da un repository remoto e le unisce con il proprio repository locale.
   
10. **`git push`**:  
    Carica le modifiche dal repository locale su un repository remoto.