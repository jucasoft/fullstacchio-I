# Get Started Cordova https://cordova.apache.org/
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
