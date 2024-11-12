## 1. Introduzione a GIT

- GIT è un sistema di controllo di versione distribuito
- Permette di gestire e tenere traccia delle modifiche apportate al codice sorgente.

## 1.1 Storia di GIT

1. **Creazione**: Git è stato creato nel 2005 da Linus Torvalds.
2. **Motivazione**: Linus cercava un sistema di controllo per sostituire "BitKeeper", utilizzato per gestire il kernel Linux.
3. **Sviluppo**: Dopo aver valutato diverse opzioni, Linus decise di creare un nuovo sistema di controllo da zero, chiamato "GIT".
4. **Nome**: Il nome "GIT" fu scelto come abbreviazione di "Global Information Tracker".
5. **Primo rilascio**: Il primo rilascio di GIT avvenne nel 2005.
6. **Popolarità**:GIT è diventato uno degli strumenti più popolari per la gestione del codice sorgente.

## 1.2 Concetto di repository

La repository di GIT è un luogo dove si memorizzano tutte le versioni del codice sorgente di un progetto. Essa ha le seguenti caratteristiche:

1. **Centralizzato**:  
   Una repository di Git è un luogo centrale dove si memorizzano tutte le versioni del codice sorgente.
2. **Versionato**:  
   Una repository contiene tutte le versioni del codice sorgente, quindi è possibile ripristinare una versione precedente se necessario.
3. **Distribuito**:  
   Una repository di Git può essere distribuito su più computer, permettendo a più persone di lavorare sullo stesso progetto contemporaneamente.
4. **Ramificato**:  
   Una repository di Git consente di creare rami (branch) per lavorare su diverse versioni del codice sorgente contemporaneamente.

## 1.3 Comandi base di GIT

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

## 2. Spiegazione di comandi avanzati

## 2.1 `git diff`

Il comando `git diff` viene utilizzato per visualizzare le differenze tra le varie versioni del codice. Può mostrare le modifiche non ancora aggiunte all'indice (`staged area`) o le differenze tra vari rami, commit, ecc.

**Differenze tra l'area di lavoro e l'indice (staged area):**

```bash
git diff
```

**Differenze tra l'indice e l'ultimo commit:**

```bash
git diff --cached
```

**Differenze tra due commit:**

```bash
git diff commit1 commit2
```

## 2.2 git stash

Il comando git stash consente di salvare temporaneamente le modifiche non commesse nell'area di lavoro e di tornare a un'area di lavoro pulita. È utile quando si desidera passare a un'altra attività senza commettere le modifiche attuali.

**Salvare le modifiche:**

```bash
git stash
```

**Visualizzare gli stashes:**

```bash
git stash list
```

**Applicare e rimuovere l'ultimo stash:**

```bash
git stash pop
```

**Applicare l'ultimo stash:**

```bash
git stash apply
```

## 2.3 git Reset

Il comando git reset viene utilizzato per annullare i cambiamenti. Può essere utilizzato per modificare l'indice o per ripristinare completamente un repository a uno stato precedente.7

**Resettare l'indice e mantenere le modifiche nell'area di lavoro:**

```bash
git reset
```

**Resettare l'indice e l'area di lavoro a uno stato precedente:**

```bash
git reset --hard commit
```

## 2.4 git checkout

Il comando git checkout viene utilizzato per spostarsi tra i rami o per ripristinare i file dall'indice o da un commit specifico.

**Passare a un altro ramo:**

```bash
git checkout branch-name
```

**Creare un nuovo ramo e passare ad esso:**

```bash
git checkout -b new-branch-name
```

**Ripristinare un file specifico da un commit:**

```bash
git checkout commit -- path/to/file
```

## 2.5 git tag

Il comando git tag viene utilizzato per creare tag che sono marcatori per commit specifici. Sono spesso usati per segnare versioni di release.

**Creare un tag annotato:**

```bash
git tag -a v1.0 -m "Versione 1.0"
```

**Elencare i tag:**

```bash
git tag
```

**Pusheare un tag remoto:**

```bash
git push origin tagname
```

\*\*Eliminare un tag locale:

```bash
git tag -d tagname
```

**Eliminare un tag remoto:**

```bash
git push origin --delete tag tagname
```

# 3. Differenze tra i vari metodi di commit in Git

## 3.1 Commit Normali

Un commit normale è il metodo standard per registrare le modifiche nel repository Git. Ogni commit ha un messaggio che descrive le modifiche e un hash univoco che lo identifica.

### Esempio

```bash
git add file.txt
git commit -m "Aggiunge modifiche al file.txt"
```

## 3.2 Git commit amend

Il comando --amend consente di modificare l'ultimo commit. Questo è utile per correggere errori nel messaggio di commit o per aggiungere nuove modifiche che dovrebbero essere incluse nell'ultimo commit.

**Esempio: Modifica del messaggio di commit**

```bash
git commit --amend -m "Nuovo messaggio per l'ultimo commit"
```

**Esempio: Aggiungere modifiche all'ultimo commit**

```bash
git add file2.txt
git commit --amend
```

## 3.3 git rebase

Il comando rebase permette di riscrivere la cronologia dei commit. È utile per mantenere una cronologia di commit lineare e pulita.

**Esempio: Rebase interattivo**

```bash
git rebase -i HEAD~3
```

**Esempio: Applicare i commit di un ramo sopra un altro**

```bash
git checkout feature-branch
git rebase main
```

## 3.4 git cherry-pick

Il comando cherry-pick consente di applicare un singolo commit da un ramo ad un altro. È utile per applicare specifiche modifiche senza dover unire interi rami.

## Esempio

```bash
git cherry-pick commit-hash
```

## 3.5 git revert

Il comando revert crea un nuovo commit che annulla le modifiche di un commit precedente. È utilizzato per mantenere la cronologia di commit intatta pur annullando le modifiche.

## Esempio

```bash
git revert commit-hash
```

## 3.6 git reset

Il comando reset viene utilizzato per spostare l'HEAD a un commit specificato, modificando l'indice e l'area di lavoro.

**Esempio: Reset soft**

```bash
git reset --soft HEAD~1
```

**Esempio: Reset hard**

```bash
git reset --hard HEAD~1
```

# 4. Differenza tra i vari tipi di merge in Git

In Git, ci sono diversi metodi per integrare le modifiche da un ramo all'altro. I principali metodi di merge sono `merge`, `squash merge`, e `rebase`. Ognuno di questi ha caratteristiche specifiche e si adatta a diverse situazioni.

## 4.1 Merge

Un merge standard in Git unisce due rami creando un nuovo commit di merge. Questo tipo di merge conserva la cronologia di entrambi i rami e crea una nuova cronologia a partire dal punto di unione.

### Esempio

```bash
git checkout main
git merge feature-branch
```

**Caratteristiche**

- Cronologia preservata: Conserva la cronologia di entrambi i rami, inclusi tutti i commit individuali.
- Commit di merge: Crea un commit di merge che indica la fusione dei due rami.
  **Vantaggi**
- Storia completa: Mantiene una traccia completa di tutte le modifiche e di come sono state integrate.
- Facilità di tracking: È facile vedere dove i rami sono stati uniti.
  **Svantaggi**
- Cronologia più complessa: La cronologia può diventare più difficile da seguire con molti commit di merge.

## 4.2 Squash Merge

Un squash merge combina tutti i commit di un ramo in un singolo commit e poi lo unisce al ramo di destinazione. Questo metodo è utile per mantenere una cronologia più pulita e comprensibile.

## Esempio

```bash
git checkout main
git merge --squash feature-branch
git commit -m "Merges feature-branch with squashed commits"
```

**Caratteristiche**

- Commits squashed: Combina tutti i commit del ramo in un unico commit.
- Commit singolo: Unisce il ramo con un singolo commit che rappresenta tutte le modifiche.
  **Vantaggi**
- Cronologia pulita: Mantiene una cronologia più lineare e pulita.
- Chiarezza: Un singolo commit rappresenta tutte le modifiche del ramo, rendendo più facile capire cosa è stato fatto.
  **Svantaggi**
- Perdita di dettagli: Perde la cronologia dettagliata dei singoli commit nel ramo unito.

## 4.3 Rebase

Il rebase sposta o riapplica i commit di un ramo su un altro, creando una cronologia lineare. Invece di unire i rami con un commit di merge, il rebase riscrive la cronologia del ramo.

## Esempio

```bash
git checkout feature-branch
git rebase main
```

**Caratteristiche**

- Cronologia riscritta: Riapplica i commit del ramo corrente sul ramo di base.
- Cronologia lineare: Crea una cronologia lineare senza commit di merge.
  **Vantaggi**
- Cronologia pulita e lineare: Facilita la lettura e la comprensione della cronologia dei commit.
- Nessun commit di merge: Non crea commit di merge, evitando la complessità aggiuntiva nella cronologia.
  **Svantaggi**
- Rischi di riscrittura: Può essere rischioso riscrivere la cronologia condivisa, causando potenziali conflitti.
- Conflitti di merge: I conflitti devono essere risolti durante il rebase, il che può essere più complesso.
