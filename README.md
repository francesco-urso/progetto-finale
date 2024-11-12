# Presentazione del Progetto

Questo progetto è una guida all'uso di **Git** e **GitHub** per la gestione del controllo di versione e della collaborazione nei progetti software. Qui troverai risorse dettagliate per imparare ad utilizzare Git e GitHub, insieme alle istruzioni di configurazione e installazione necessarie per iniziare.

## Contenuto del Progetto

- **Introduzione a Git**  
  Troverai una guida all'interno del file [GIT.md](./GIT.md), con spiegazioni su come utilizzare i comandi principali di Git, creare branch, gestire il flusso di lavoro e sincronizzarsi con i repository remoti.

- **Introduzione a GitHub**  
  La guida su GitHub, disponibile in [GITHUB.md](./GITHUB.md), copre le funzionalità principali della piattaforma, tra cui la creazione di repository, issue, pull request e l'uso delle milestone per l'organizzazione delle task e del lavoro di gruppo.

- **Installazione di Git**  
  Per iniziare ad utilizzare Git, consulta la sezione seguente:

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
