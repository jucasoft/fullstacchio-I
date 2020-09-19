# Introduzione
Con il passare del tempo, trovare il tempo per riuscire a studiare nuove tecnologie è sempre meno, l'idea di questo corso è di darvi un percorso guidato costituito dai migliori tutorial trovati in rete, un strada sicura, che vi porterà ad attraversare i concetti fondamentali della programmazione Fullstacchia (Angular).


# Linee guida
Ogni esercizio dovrà essere committato su GitHub.

L'IDE da utilizzare è intellij Ultimate Trial.

Il periodo di prova di Intellij avvolte scade in modo imprevisto, in questo caso riavviate il pc e utilizzare un .bat con il seguente codice:
    
```
cd "C:%HOMEPATH%\.IntelliJIdea*\config"
rmdir "eval" /s /q
del "options\other.xml"
reg delete "HKEY_CURRENT_USER\Software\JavaSoft\Prefs\jetbrains\idea" /f
```

In caso di difficolta nello svolgimento dei tutorial aprite una Issue in GitHub, indicando più informazioni possibili:

# Le basi  
## 1) Getting started https://angular.io/guide/setup-local
In questa pagina si trova il tutorial per creare il primo progetto in Angular, al termine di questo tutorial sarete in grado di preparare l'ambiente di sviluppo per creare un'applicazione in Angular.

Argomenti trattati:
- NodeJs
- npm
- Angular CLI

Dopo avere creato il progetto (anche se non funzionante), caricare il codice su GitLab:
- entrare nella cartella del progetto creato e cancellare la cartella ".git"
- posizionarsi sulla pagina principale di https://gitlab.com
- click su "New Project"
- compilare il campo "Project name" con "NG Getting started"
- click su "Create project"
- scorrere la pagina fino a trovare la sezione "Push an existing folder"
- eseguire i comandi presenti (da verificare)

Condividere il progetto:
- aprire il progetto in GitLab
- cliccare sulla voce di menù "Settings" -> "Members"
- nel campo "Select members to invite" scrivere il nome utente.
- aggiungertemi come "Developer"


## 2) Tour of Heroes https://angular.io/
Il tutorial permetterà di affrontare gli aspetti principali di Angular.

## 3) Struttura del progetto, dove metto cosa.
La struttura di un progetto è una di quelle cose che può dare grandi soddisfazioni, non possiamo ogni volta inventarci un posto dove mettere i nostri file; Angular crea già una serie di cartelle, ma non basta, dobbiamo adottare una metologia che possa andare bene dall'inizio alla fine del nostro progetto. Come un buon pizzaiolo prepara gli alimenti per sapere sepre dove trovarli, anche noi dobbiamo avere sempre la stessa metologia, che si ripete.
```
- src
  - app (cartella generata in automatico da Angular)
    - core
      - components
      - models
        - vo
        - api
      - services
      - utilities
    - main
      - components
      - models
        - vo
        - api
      - pages
      - services 
```
### core
In questa cartella metteremo tutte quelle entità/componenti..., che non hanno dipendenza stretta con il dominio del progetto.
Alcuni di questi file potranno diventare delle librerie comuni tra vari progetti.
Ad esempio: ServiceBase (che verrà estesa da tutti i miei servizi), HeaderComponent (componente generico che rappresenterà header dell'applicazione), ...

### main
Questo è il punto dove si trovano tutti i file che fanno riferimento al dominio dell'applicazione.
Per questa parte vi chiederei di farmi degli esempi per vedere se avete capito e se siete sttati così pazienti dal leggeri sta roba.


# 4) Get Started Cordova https://cordova.apache.org/
La prima APP (Android/IOS/WEB) ibrida.
Armatevi di pazienza e tanti GIGHI, scaricare le sdk Android è un lungo e doloroso viaggio.
Ad oggi ha vinto Angelo, con i suoi 17 tentativi e tutta la banda di Iliad fatta fuori.

## Avete scaricato le SDK ma non riuscite ad avviare la macchina virtuale
Grazie agli alunni che vi hanno preceduto, abbaimo selezionato gli ostacoli maggiori nella riuscita di questo punto didattico.

### SDK android non viene scaricata completamente.
- chiudere AndroidStudio
- riaprire AndroidStudio
- andare nella gestione sdk, cliccare sul link "edit" accanto al percorso dove si trovano le sdk
- lasciare tutto predefinito e procedere
- la procedura d'installazione finisce immediatamente e permette di chiudere la procedura correttamente (in precedenza bloccandosi era stato killato)

### Accelleratore grafico non è stato installato realmente (un grazie ad Antorio).
- andare nella gestione sdk sezione tools
- disinstallare: "Intel® Hardware Accelerated Execution Manager (Intel® HAXM)",  disinstallandola segnala che in realtà non è presente e non può rimuoverla
- selezionare la voce appena rimossa e procedere per reinstallarla


# 5) [Nodejs, Express, Mongodb](https://medium.com/@dinyangetoh/how-to-build-simple-restful-api-with-nodejs-expressjs-and-mongodb-99348012925d)
Questo tutorial mi piace parecchio, spiega come poter realizzare servizi con js, un solo linguaggio per BE/FE/FF.


# Quando il gioco si fa duro 
Se sei riuscito ad arrivare indenne a questo punto potrai accedere al nuovo livello.
https://www.engiel.com/wp-content/uploads/2018/07/gif-applauso-2.gif
