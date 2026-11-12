<p align="center">
  <img src="https://dynamicdnspro.com/assets/img/logo.png" alt="Dynamic DNS Pro" width="96">
</p>

<h1 align="center">DDNSPro Remote</h1>

<p align="center">Ihre Rechner, einen Klick entfernt.<br>Sicherer WebRTC-Fernzugriff — nativer Viewer für macOS, Remote-Host für Windows.</p>

<p align="center">
  <a href="https://remote.dynamicdnspro.com"><img src="https://img.shields.io/badge/website-remote.dynamicdnspro.com-0A84FF" alt="website"></a>
  <a href="https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest"><img src="https://img.shields.io/github/v/release/mavksoft/dynamicdnspro-remote-releases?label=latest" alt="latest release"></a>
  <img src="https://img.shields.io/badge/platform-macOS%20%C2%B7%20Windows-black" alt="platforms">
  <img src="https://img.shields.io/badge/license-commercial-orange" alt="commercial license">
</p>

<p align="center"><a href="https://mavksoft.github.io/dynamicdnspro-remote-releases/"><img src="https://img.shields.io/static/v1?label=docs&message=mavksoft.github.io/dynamicdnspro-remote-releases&color=blue" alt="docs"></a></p>

<p align="center">🌍 <a href="README.es.md">🇪🇸 Español</a> · <a href="README.md">🇬🇧 English</a> · <strong>🇩🇪 Deutsch</strong> · <a href="README.fr.md">🇫🇷 Français</a> · <a href="README.it.md">🇮🇹 Italiano</a> · <a href="README.pt.md">🇵🇹 Português</a></p>

> **Dieses Repository veröffentlicht ausschließlich offizielle Binär-Releases** — der Quellcode ist privat. Signierte Downloads, Prüfsummen und Auto-Update-Feeds.

## Download

| | |
|---|---|
| <img src='https://raw.githubusercontent.com/mavksoft/dynamicdnspro-remote-releases/main/icons/apple.svg' width='15' style='vertical-align:-2px' alt='apple'> **Viewer (macOS)** | [DDNSProRemote-macOS.dmg](https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest) — nativer Client, Developer-ID-signiert und notarisiert |
| <img src='https://raw.githubusercontent.com/mavksoft/dynamicdnspro-remote-releases/main/icons/windows.svg' width='15' style='vertical-align:-2px' alt='windows'> **Remote-Host (Windows)** | [DynamicDNSPro-Remote-Setup.exe](https://github.com/mavksoft/dynamicdnspro-releases/releases/latest) — auf den Rechnern installieren, die Sie erreichen möchten |
| <img src='https://dynamicdnspro.com/assets/img/logo.png' width='15' style='vertical-align:-2px'> **Web-Viewer** | [remote.dynamicdnspro.com](https://remote.dynamicdnspro.com) — vollständige Sitzungen aus jedem Browser, ohne Installation |
| <img src='https://dynamicdnspro.com/assets/img/logo.png' width='15' style='vertical-align:-2px'> **Website** | [dynamicdnspro.com](https://dynamicdnspro.com) — Kundenportal, Pläne und FAQ |

## Was ist das

DDNSPro Remote ist das Fernzugriffs-Produkt des Dynamic-DNS-Pro-Ökosystems — separat lizenziert, aber mit gemeinsamem Konto, Maschinen und Berechtigungen mit dem Webportal. Installieren Sie den Host auf den verwalteten Rechnern und greifen Sie über den nativen macOS-Viewer oder einen beliebigen Browser zu: Desktop, Dateien, Konsole und Energieaktionen über Ende-zu-Ende-verschlüsseltes WebRTC.

<p align="center"><img src="./screenshots/website.png" width="640" alt="screenshot"></p>

## Funktionen

- **WebRTC-P2P-Sitzungen** — Desktop-Video, Audio und Eingabe mit geringer Latenz, DTLS Ende zu Ende verschlüsselt.
- **Zugriff mit Zustimmung** — die Gegenseite bestätigt jede Sitzung (oder Sie vergeben pro Rechner eine dauerhafte/Wiederverbindungs-Freigabe).
- **Dateimanager & Transfer** — Remote-Laufwerke durchsuchen, Up-/Downloads per Drag & Drop direkt in der Sitzung.
- **Maschinen-Lobby** — Ihre Rechner mit Live-Miniaturen, oder Ad-hoc-Verbindungen per ID + Passwort.
- **RDP-Sitzungswahl** — auf Multi-Session-Hosts eine bestehende Sitzung wählen oder eine neue öffnen.
- **Auflösungssteuerung** — Remote-Auflösung im laufenden Betrieb wechseln (Admin-Profile).
- **Warten auf Wiederverbindung** — Remote-Neustart: die Sitzung wartet und verbindet sich von selbst wieder.
- **Energieaktionen** — Neustart, Sperren, Strg+Alt+Entf / SAS, Win+D aus der Sitzungsleiste.
- **Zwischenablage, Remote-Cursor, Tastatur & Maus** — volle Eingabe-Parität mit dem Web-Viewer.
- **Signierte Auto-Updates** — Ed25519-signierte Manifeste; macOS-Builds von Apple notarisiert.
- **Sechs Sprachen** — ES / EN / FR / IT / DE / PT.

## So funktioniert es

1. Registrieren Sie sich auf [dynamicdnspro.com](https://dynamicdnspro.com) und aktivieren Sie einen Remote-Plan.
2. Installieren Sie auf jedem Zielrechner den **Windows-Remote-Host** — er meldet sich mit einer Maschinen-ID unter Ihrem Konto an.
3. Legen Sie die Zugriffsrichtlinie pro Rechner fest: immer Zustimmung, immer erlauben oder mit Kulanzzeit für Wiederverbindung.
4. Öffnen Sie den **macOS-Viewer** (oder die Web-Lobby) und melden Sie sich an — Ihre Rechner erscheinen mit Live-Status.
5. Klick auf einen Rechner → Sitzung öffnet sich: Desktop, Dateien und Energieaktionen in einem Fenster.

## Inhalt dieses Repositories

- `DDNSProRemote-macOS-<Version>.dmg` — macOS-Viewer-Installer (Developer ID + notarisiert)
- `DDNSProRemote-macOS-<Version>.zip` — Update-Paket für den integrierten Updater
- `visor_macos.json` — signiertes Versionsmanifest (Ed25519) für den Auto-Updater
- `visor_macos_appcast.xml` — Legacy-Sparkle-Feed für Installationen vor 1.1.0
- `*.sha256` — Prüfsummen für jede Binärdatei

[Aktuelles Release](https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest)

## FAQ

**Ist der Datenverkehr verschlüsselt?**
Ja — Sitzungen laufen über WebRTC mit DTLS-SRTP; das Signalisieren erfolgt über authentifiziertes TLS. Nichts wird im Klartext übertragen, Zustimmung/Richtlinien werden hostseitig durchgesetzt.

**Brauche ich ein Dynamic-DNS-Pro-Abo?**
Remote wird separat lizenziert — Sie können es eigenständig erwerben. Mit bestehendem Konto teilen sich beide Login und Maschinenliste.

**Unterschied zwischen Viewer und Host?**
Der Viewer (dieses Repo) läuft bei *Ihnen* zum Verbinden; der Host (in `dynamicdnspro-releases`) läuft auf dem entfernten Rechner.

**Verbindung ohne Konto möglich?**
Ja — Ad-hoc-Sitzungen funktionieren mit ID und Passwort des Remote-Rechners, wie bei klassischen Support-Tools.

## Support

- Website & Kundenportal: [dynamicdnspro.com](https://dynamicdnspro.com)
- Remote-Web-Lobby: [remote.dynamicdnspro.com](https://remote.dynamicdnspro.com)
- E-Mail: support@it-systems.es

---
<p align="center"><sub>DDNSPro Remote · © MavkSoft / IT-Systems</sub></p>
