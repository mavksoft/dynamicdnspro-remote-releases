<p align="center">
  <img src="https://dynamicdnspro.com/assets/img/logo.png" alt="Dynamic DNS Pro" width="96">
</p>

<h1 align="center">DDNSPro Remote</h1>

<p align="center">Le tue macchine, a un clic.<br>Desktop remoto WebRTC sicuro — visualizzatore nativo per macOS, host remoto per Windows.</p>

<p align="center">
  <a href="https://remote.dynamicdnspro.com"><img src="https://img.shields.io/badge/website-remote.dynamicdnspro.com-0A84FF" alt="website"></a>
  <a href="https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest"><img src="https://img.shields.io/github/v/release/mavksoft/dynamicdnspro-remote-releases?label=latest" alt="latest release"></a>
  <img src="https://img.shields.io/badge/platform-macOS%20%C2%B7%20Windows-black" alt="platforms">
  <img src="https://img.shields.io/badge/license-commercial-orange" alt="commercial license">
</p>

<p align="center"><a href="https://mavksoft.github.io/dynamicdnspro-remote-releases/"><img src="https://img.shields.io/static/v1?label=docs&message=mavksoft.github.io/dynamicdnspro-remote-releases&color=blue" alt="docs"></a></p>

<p align="center">🌍 <a href="README.es.md">🇪🇸 Español</a> · <a href="README.md">🇬🇧 English</a> · <a href="README.de.md">🇩🇪 Deutsch</a> · <a href="README.fr.md">🇫🇷 Français</a> · <strong>🇮🇹 Italiano</strong> · <a href="README.pt.md">🇵🇹 Português</a></p>

> **Questo repository pubblica solo release binarie ufficiali** — il codice sorgente è privato. Download firmati, checksum e feed di auto-aggiornamento.

## Download

| | |
|---|---|
| <img src='https://raw.githubusercontent.com/mavksoft/dynamicdnspro-remote-releases/main/icons/apple.svg' width='15' style='vertical-align:-2px' alt='apple'> **Visualizzatore (macOS)** | [DDNSProRemote-macOS.dmg](https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest) — client nativo, firmato Developer ID e notarizzato |
| <img src='https://raw.githubusercontent.com/mavksoft/dynamicdnspro-remote-releases/main/icons/windows.svg' width='15' style='vertical-align:-2px' alt='windows'> **Host remoto (Windows)** | [DynamicDNSPro-Remote-Setup.exe](https://github.com/mavksoft/dynamicdnspro-releases/releases/latest) — da installare sulle macchine da raggiungere |
| <img src='https://dynamicdnspro.com/assets/img/logo.png' width='15' style='vertical-align:-2px'> **Visualizzatore web** | [remote.dynamicdnspro.com](https://remote.dynamicdnspro.com) — sessioni complete da qualsiasi browser, senza installazione |
| <img src='https://dynamicdnspro.com/assets/img/logo.png' width='15' style='vertical-align:-2px'> **Sito ufficiale** | [dynamicdnspro.com](https://dynamicdnspro.com) — portale clienti, piani e FAQ |

## Cos'è

DDNSPro Remote è il prodotto di accesso remoto dell'ecosistema Dynamic DNS Pro — con licenza separata, ma condividendo account, macchine e permessi con il portale web. Installa l'host sulle macchine che gestisci e raggiungile dal visualizzatore macOS nativo o da qualsiasi browser: desktop, file, console e azioni di alimentazione su WebRTC cifrato end-to-end.

<p align="center"><img src="./screenshots/website.png" width="640" alt="screenshot"></p>

## Funzionalità

- **Sessioni WebRTC P2P** — video desktop, audio e input a bassa latenza con cifratura DTLS end-to-end.
- **Accesso con consenso** — il lato remoto approva ogni sessione (o permesso permanente/di riconnessione per macchina).
- **Gestore file** — sfoglia le unità remote, upload e download con drag & drop dentro la sessione.
- **Lobby macchine** — le tue macchine con miniature live, o connessioni ad-hoc con ID + password.
- **Selettore sessione RDP** — su host multi-sessione, scegli una sessione esistente o aprine una nuova.
- **Controllo risoluzione** — cambia la risoluzione remota a caldo (profili admin).
- **Attesa di riconnessione** — riavvia la macchina remota: la sessione aspetta e si riaggancia da sola.
- **Azioni di alimentazione** — riavvio, blocco, Ctrl+Alt+Canc / SAS, Win+D dalla barra di sessione.
- **Appunti, cursore remoto, tastiera e mouse** — parità totale di input con il visualizzatore web.
- **Auto-aggiornamenti firmati** — manifest Ed25519; build macOS notarizzate da Apple.
- **Sei lingue** — ES / EN / FR / IT / DE / PT.

## Come si usa

1. Registrati su [dynamicdnspro.com](https://dynamicdnspro.com) e attiva un piano Remote.
2. Su ogni macchina da raggiungere, installa l'**host Remote per Windows** — si registra sul tuo account con un ID macchina.
3. Definisci la politica di accesso per macchina: consenso ogni volta, sempre consentito, o consentito con periodo di grazia per la riconnessione.
4. Apri il **visualizzatore macOS** (o la lobby web), accedi — le tue macchine appaiono con lo stato live.
5. Clic su una macchina → si apre la sessione: desktop, file e azioni di alimentazione in una sola finestra.

## Contenuto di questo repository

- `DDNSProRemote-macOS-<versione>.dmg` — installer del visualizzatore macOS (Developer ID + notarizzato)
- `DDNSProRemote-macOS-<versione>.zip` — pacchetto di aggiornamento per l'updater integrato
- `visor_macos.json` — manifest di versione firmato (Ed25519) letto dall'auto-updater
- `visor_macos_appcast.xml` — feed Sparkle legacy per installazioni precedenti alla 1.1.0
- `*.sha256` — checksum di ogni binario

[Ultima release](https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest)

## FAQ

**Il traffico è cifrato?**
Sì — le sessioni viaggiano su WebRTC con DTLS-SRTP; la segnalazione passa su TLS autenticato. Nulla transita in chiaro e consenso/politiche sono applicati lato host.

**Serve un abbonamento Dynamic DNS Pro?**
Remote ha licenza separata — puoi acquistarlo da solo. Se hai già un account, condivide login e lista macchine.

**Differenza tra visualizzatore e host?**
Il visualizzatore (questo repo) è ciò che *tu* esegui per connetterti; l'host (in `dynamicdnspro-releases`) gira sulla macchina remota.

**Posso connettermi senza account?**
Sì — le sessioni ad-hoc funzionano con ID e password della macchina remota, come i classici strumenti di assistenza.

## Supporto

- Sito e portale clienti: [dynamicdnspro.com](https://dynamicdnspro.com)
- Lobby web Remote: [remote.dynamicdnspro.com](https://remote.dynamicdnspro.com)
- Email: support@it-systems.es

---
<p align="center"><sub>DDNSPro Remote · © MavkSoft / IT-Systems</sub></p>
