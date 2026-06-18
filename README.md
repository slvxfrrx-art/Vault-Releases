# Vault

Vault è un’applicazione desktop per Windows progettata per gestire in modo sicuro credenziali, connessioni VPN, sistemi SAP, allegati, configurazioni tecniche e spazi di collaborazione cifrati.

Questo repository pubblico contiene esclusivamente:

* installer ufficiali;
* file necessari agli aggiornamenti automatici;
* firme degli aggiornamenti;
* note di rilascio;
* documentazione pubblica essenziale.

Il codice sorgente privato dell’applicazione non è pubblicato in questo repository.

---

## Ultima versione

### Vault v1.4.0

**Themes and Interface Personalization**

La versione 1.4.0 introduce:

* modalità chiara e scura;
* possibilità di seguire automaticamente il tema di Windows;
* temi grafici preimpostati;
* personalizzazione di colori, pulsanti, pannelli, bordi e sfondi;
* supporto per immagini di sfondo locali;
* controllo del contrasto e recupero automatico in caso di tema non valido;
* interfaccia multilingua;
* miglioramenti al Team Workspace;
* gestione semplificata dei Team;
* miglioramenti alla procedura di aggiornamento.

---

## Download

Per una normale installazione su Windows è consigliato il file:

```text
Vault_1.4.0_x64-setup.exe
```

È disponibile anche il pacchetto MSI:

```text
Vault_1.4.0_x64_en-US.msi
```

I file `.sig` vengono utilizzati da Vault per verificare l’autenticità degli aggiornamenti automatici.

Il file:

```text
latest.json
```

contiene le informazioni necessarie al sistema di aggiornamento integrato.

---

## Funzionalità principali

### Vault locale

Vault consente di archiviare e organizzare:

* credenziali;
* utenti e password;
* connessioni VPN;
* connessioni SAP e altri sistemi;
* host, porte, client e parametri tecnici;
* più utenti per ogni connessione;
* allegati;
* loghi;
* note;
* cronologia delle modifiche;
* cartelle e sottocartelle;
* backup e ripristino.

I dati locali vengono protetti all’interno del Vault dell’utente.

---

### Team Collaboration

Vault permette di creare spazi Team condivisi e cifrati.

Le funzionalità Team includono:

* membri;
* ruoli;
* permessi;
* dispositivi approvati;
* inviti firmati;
* cartelle logiche condivise;
* allegati cifrati;
* eventi firmati;
* gestione dei conflitti;
* snapshot;
* backup Team;
* revoca dei dispositivi;
* rotazione delle chiavi;
* verifica dello stato di sincronizzazione;
* registro delle attività;
* riconciliazione degli accessi.

L’accesso alla cartella condivisa e l’accesso ai dati Vault restano separati.

Un utente che può vedere i file cifrati nel servizio cloud non può automaticamente decifrare il contenuto del Team.

---

## Posizioni supportate per i Team

Vault può utilizzare:

* Microsoft OneDrive;
* cartelle SharePoint sincronizzate;
* Google Drive for desktop;
* Microsoft 365 tramite account collegato;
* Google Drive tramite account collegato;
* cartelle aziendali di rete;
* unità di rete mappate;
* cartelle locali;
* altri servizi di sincronizzazione accessibili da Windows.

Per i nuovi Team su OneDrive viene utilizzata una struttura leggibile:

```text
OneDrive\Vault\Nome Team
```

La struttura fisica contiene file cifrati e dati tecnici.

Le cartelle operative del Team vengono invece mostrate direttamente nel **Team Workspace** di Vault.

---

## Microsoft 365 e Google Drive

Il collegamento degli account Microsoft e Google è facoltativo.

Quando disponibile, Vault può:

* creare la cartella Team;
* verificare l’accesso;
* condividere la cartella con un collaboratore;
* controllare lo stato della condivisione;
* rimuovere l’accesso quando un collaboratore lascia il Team.

È sempre disponibile una modalità manuale basata su cartelle già sincronizzate nel PC.

Le policy aziendali di Microsoft 365 o Google Workspace possono limitare alcune operazioni di condivisione.

---

## Lingue disponibili

Vault supporta:

* Italiano;
* English;
* Français;
* Español;
* Deutsch.

La lingua può essere modificata da:

```text
Impostazioni → Aspetto e lingua
```

La modifica viene applicata senza alterare i dati archiviati.

---

## Aspetto e temi

Vault supporta:

* Segui Windows;
* Tema chiaro;
* Tema scuro;
* Vault Light;
* Vault Dark;
* Vault Blue;
* Vault Green;
* Vault Purple;
* Vault Graphite;
* Alto contrasto;
* Tema personalizzato.

La personalizzazione può includere:

* colore principale;
* colore secondario;
* sfondo;
* pannelli;
* pulsanti;
* testo;
* bordi;
* angoli;
* ombre;
* trasparenza;
* immagine di sfondo locale.

Le preferenze grafiche sono locali e non vengono condivise nei Team.

---

## Sicurezza

Vault utilizza un modello di sicurezza separato dal servizio cloud utilizzato per la sincronizzazione.

Principi principali:

* i dati Team vengono cifrati prima di essere salvati;
* i dispositivi devono essere approvati;
* gli eventi Team vengono firmati;
* ogni dispositivo dispone delle proprie chiavi;
* le chiavi Team vengono distribuite tramite keybox dedicate;
* i membri rimossi non ricevono le nuove chiavi dopo la rotazione;
* gli allegati Team vengono archiviati cifrati;
* backup e snapshot Team restano cifrati;
* i token Microsoft e Google rimangono locali;
* token e credenziali cloud non vengono inseriti nei file Team;
* non vengono creati link pubblici anonimi per impostazione predefinita.

La rimozione di un membro impedisce l’accesso futuro dopo la rotazione delle chiavi.

Non è tecnicamente possibile cancellare da remoto informazioni già visualizzate, esportate o copiate da un utente autorizzato.

---

## Nessun server dedicato richiesto

Il funzionamento standard di Vault e dei Team non richiede:

* VPS;
* server applicativo;
* PostgreSQL;
* FastAPI;
* Docker;
* servizi backend dedicati.

La collaborazione può funzionare attraverso una cartella condivisa o sincronizzata.

---

## Aggiornamenti automatici

Vault controlla gli aggiornamenti attraverso questo repository pubblico.

Endpoint utilizzato:

```text
https://github.com/slvxfrrx-art/Vault-Releases/releases/latest/download/latest.json
```

Gli aggiornamenti vengono verificati tramite firma prima dell’installazione.

Per il corretto funzionamento devono essere presenti nella release:

```text
Vault_<versione>_x64-setup.exe
Vault_<versione>_x64-setup.exe.sig
Vault_<versione>_x64_en-US.msi
Vault_<versione>_x64_en-US.msi.sig
latest.json
```

---

## Requisiti

* Windows 10 o successivo;
* architettura x64;
* spazio disponibile per installazione, dati e allegati;
* connessione Internet solo per:

  * aggiornamenti;
  * collegamento account cloud;
  * sincronizzazione tramite servizi online.

Il Vault locale può essere utilizzato senza connessione Internet.

---

## Installazione

1. Scarica l’installer EXE o MSI dalla sezione **Releases**.
2. Avvia il file.
3. Completa l’installazione.
4. Apri Vault.
5. Crea un nuovo Vault oppure ripristina un backup esistente.

Windows SmartScreen potrebbe mostrare un avviso per release nuove o con reputazione ancora limitata.

Controlla sempre che il file provenga dal repository ufficiale:

```text
slvxfrrx-art/Vault-Releases
```

---

## Aggiornamento da una versione precedente

Prima di aggiornare è consigliato creare un backup.

L’aggiornamento mantiene:

* dati locali;
* Team;
* cartelle;
* connessioni;
* allegati;
* impostazioni;
* preferenze linguistiche;
* preferenze grafiche.

Le funzionalità Team e gli account cloud restano facoltativi.

---

## Limitazioni note

* le operazioni cloud dipendono dalla disponibilità del provider;
* le organizzazioni possono bloccare la condivisione esterna;
* alcune autorizzazioni potrebbero richiedere un intervento manuale;
* le cartelle di rete dipendono dall’accesso Windows corrente;
* la sincronizzazione può richiedere tempo;
* i permessi del servizio cloud e i permessi Vault sono separati;
* un membro rimosso potrebbe conservare dati già esportati o copiati;
* SmartScreen può mostrare un avviso sulle nuove release;
* i temi con immagini molto complesse possono richiedere un overlay per mantenere leggibili i testi.

---

## Contenuto del repository

Questo repository contiene:

```text
Installer EXE
Installer MSI
Firme updater
latest.json
README pubblico
Note di rilascio
```

Non contiene:

```text
Codice sorgente privato
Chiavi private
Credenziali
Token cloud
Dati degli utenti
Database Vault
Contenuti dei Team
```

---

## Supporto e segnalazioni

Per problemi relativi a:

* installazione;
* aggiornamenti;
* file mancanti;
* installer non avviabile;
* errori della release;

utilizza la sezione **Issues** del repository, se abilitata.

Non pubblicare mai:

* password;
* chiavi;
* token;
* backup;
* file Team;
* database;
* log contenenti informazioni riservate.

---

## Stato del progetto

Vault è sviluppato e distribuito come progetto privato.

Questo repository viene utilizzato come canale pubblico ufficiale per:

* distribuzione;
* aggiornamenti;
* documentazione essenziale;
* storico delle release.

---

## Licenza

Vault è software proprietario.

Il download dell’applicazione non concede il diritto di:

* redistribuire il codice;
* modificare il software;
* pubblicare versioni derivate;
* decompilare o riutilizzare componenti proprietari, salvo quanto consentito dalla legge applicabile.

© 2026 Vault. Tutti i diritti riservati.
