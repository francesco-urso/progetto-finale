# Presentazione del Progetto

Questo progetto è una guida all'uso di **Git** e **GitHub** per la gestione del controllo di versione e della collaborazione nei progetti software. Qui troverai risorse dettagliate per imparare ad utilizzare Git e GitHub, insieme alle istruzioni di configurazione e installazione necessarie per iniziare.

## Contenuto del Progetto

- **Introduzione a Git**  
  Troverai una guida all'interno del file [GIT.md](./GIT.md), con spiegazioni su come utilizzare i comandi principali di Git, creare branch, gestire il flusso di lavoro e sincronizzarsi con i repository remoti.

- **Introduzione a GitHub**  
  La guida su GitHub, disponibile in [GITHUB.md](./GITHUB.md), copre le funzionalità principali della piattaforma, tra cui la creazione di repository, issue, pull request e l'uso delle milestone per l'organizzazione delle task e del lavoro di gruppo.

- **Installazione di Git**  
  Per iniziare ad utilizzare Git, consulta la sezione seguente:

  ### Indice

1. [Introduzione a GIT](#1-introduzione-a-git)
   - [1.1 Storia di GIT](#11-storia-di-git)
   - [1.2 Concetto di repository](#12-concetto-di-repository)
   - [1.3 Comandi base di GIT](#13-comandi-base-di-git)
2. [Spiegazione di comandi avanzati](#2-spiegazione-di-comandi-avanzati)
   - [2.1 git diff](#21-git-diff)
   - [2.2 git stash](#22-git-stash)
   - [2.3 git reset](#23-git-reset)
   - [2.4 git checkout](#24-git-checkout)
   - [2.5 git tag](#25-git-tag)
3. [Differenze tra i vari metodi di commit in Git](#3-differenze-tra-i-vari-metodi-di-commit-in-git)
   - [3.1 Commit Normali](#31-commit-normali)
   - [3.2 Git commit amend](#32-git-commit-amend)
   - [3.3 git rebase](#33-git-rebase)
   - [3.4 git cherry-pick](#34-git-cherry-pick)
   - [3.5 git revert](#35-git-revert)
   - [3.6 git reset](#36-git-reset)
4. [Differenza tra i vari tipi di merge in Git](#4-differenza-tra-i-vari-tipi-di-merge-in-git)
   - [4.1 Merge](#41-merge)
   - [4.2 Squash Merge](#42-squash-merge)
   - [4.3 Rebase](#43-rebase)

### Installazione di Git

1. **Su Windows**:

   - Scarica il pacchetto di installazione di Git da [git-scm.com](https://git-scm.com/downloads/win).
   - Avvia l'installazione e segui le istruzioni guidate per completare l’installazione.

2. **Su macOS**:

   - Puoi installare Git usando Homebrew con il comando:

   ```bash
    brew install git
   ```

   - In alternativa, Git è disponibile anche tramite Xcode Command Line Tools.

3. **Su Linux**:

   - Su distribuzioni basate su Debian (come Ubuntu), usa:

     ```bash
     sudo apt update
     sudo apt install git
     ```

   - Su distribuzioni basate su Red Hat (come Fedora), usa:

     ```bash
     sudo dnf install git
     ```

4. **Configurazione Iniziale di Git**:

   - Dopo l'installazione, configura il tuo nome utente e la tua email:

     ```bash
     git config --global user.name "Tuo Nome"
     git config --global user.email "tuo@example.com"
     ```

   - Questi dettagli saranno inclusi nei commit che creerai.

Una volta completata l'installazione, sarai pronto per iniziare ad utilizzare Git ed inizializzare il progetto [GIT.md](./GIT.md) e GitHub per creare la tua prima repo [GITHUB.md](./GITHUB.md)

Se desideri scaricare la guida sul tuo pc puoi procedere con il comando:

- Per clonarlo nella cartela dove ti trovi:

```bash
     git clone https://github.com/francesco-urso/progetto-finale.git
```

- Per clonarlo in una directory specifica:

```bash
     git clone https://github.com/francesco-urso/progetto-finale.git /percorso/della/directory
```

# Differenza tra i vari tipi di merge in Git

In Git, ci sono diversi metodi per integrare le modifiche da un ramo all'altro. I principali metodi di merge sono `merge`, `squash merge`, e `rebase`. Ognuno di questi ha caratteristiche specifiche e si adatta a diverse situazioni.
