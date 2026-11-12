<p align="center">
  <img src="https://dynamicdnspro.com/assets/img/logo.png" alt="Dynamic DNS Pro" width="96">
</p>

<h1 align="center">DDNSPro Remote</h1>

<p align="center">Your machines, one click away.<br>Secure WebRTC remote desktop — native viewer for macOS, remote host for Windows.</p>

<p align="center">
  <a href="https://remote.dynamicdnspro.com"><img src="https://img.shields.io/badge/website-remote.dynamicdnspro.com-0A84FF" alt="website"></a>
  <a href="https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest"><img src="https://img.shields.io/github/v/release/mavksoft/dynamicdnspro-remote-releases?label=latest" alt="latest release"></a>
  <img src="https://img.shields.io/badge/platform-macOS%20%C2%B7%20Windows-black" alt="platforms">
  <img src="https://img.shields.io/badge/license-commercial-orange" alt="commercial license">
</p>

<p align="center"><a href="https://mavksoft.github.io/dynamicdnspro-remote-releases/"><img src="https://img.shields.io/static/v1?label=docs&message=mavksoft.github.io/dynamicdnspro-remote-releases&color=blue" alt="docs"></a></p>

<p align="center">🌍 <a href="README.es.md">🇪🇸 Español</a> · <strong>🇬🇧 English</strong> · <a href="README.de.md">🇩🇪 Deutsch</a> · <a href="README.fr.md">🇫🇷 Français</a> · <a href="README.it.md">🇮🇹 Italiano</a> · <a href="README.pt.md">🇵🇹 Português</a></p>

> **This repository publishes official binary releases only** — the source code is private. Signed downloads, checksums and auto-update feeds.

## Download

| | |
|---|---|
| <img src='https://raw.githubusercontent.com/mavksoft/dynamicdnspro-remote-releases/main/icons/apple.svg' width='15' style='vertical-align:-2px' alt='apple'> **Viewer (macOS)** | [DDNSProRemote-macOS.dmg](https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest) — native desktop client, Developer-ID signed & notarized |
| <img src='https://raw.githubusercontent.com/mavksoft/dynamicdnspro-remote-releases/main/icons/windows.svg' width='15' style='vertical-align:-2px' alt='windows'> **Remote host (Windows)** | [DynamicDNSPro-Remote-Setup.exe](https://github.com/mavksoft/dynamicdnspro-releases/releases/latest) — install this on the machines you want to reach |
| <img src='https://dynamicdnspro.com/assets/img/logo.png' width='15' style='vertical-align:-2px'> **Web viewer** | [remote.dynamicdnspro.com](https://remote.dynamicdnspro.com) — full sessions from any browser, no install |
| <img src='https://dynamicdnspro.com/assets/img/logo.png' width='15' style='vertical-align:-2px'> **Website** | [dynamicdnspro.com](https://dynamicdnspro.com) — client portal, plans and FAQ |

## What it is

DDNSPro Remote is the remote-access product of the Dynamic DNS Pro ecosystem — separately licensed, sharing your account, machines and permissions with the web portal. Install the host on the machines you manage, then reach them from the native macOS viewer or any browser: desktop, files, console and power actions over end-to-end-encrypted WebRTC.

<p align="center"><img src="./screenshots/website.png" width="640" alt="screenshot"></p>

## Features

- **WebRTC P2P sessions** — low-latency desktop video, audio and input with DTLS encryption end to end.
- **Consent-based access** — the remote side approves each session (or you grant a permanent/reconnect allowance per machine).
- **File manager & transfer** — browse remote drives, drag-and-drop uploads and downloads inside the session.
- **Machine lobby** — your account machines with live thumbnails, or ad-hoc connections by ID + password.
- **RDP session picker** — on multi-session hosts, choose an existing session or open a new one.
- **Resolution control** — switch the remote display resolution in-session (admin profiles).
- **Wait-for-reconnect** — reboot the remote machine and the session waits and reattaches on its own.
- **Power actions** — reboot, lock screen, Ctrl+Alt+Del / SAS, Win+D from the session bar.
- **Clipboard sync, remote cursor, keyboard & mouse** — full input parity with the web viewer.
- **Signed auto-updates** — Ed25519-signed manifests; macOS builds are notarized by Apple.
- **Six languages** — ES / EN / FR / IT / DE / PT.

## How to use it

1. Sign up at [dynamicdnspro.com](https://dynamicdnspro.com) and enable a Remote plan.
2. On each machine you want to reach, install the **Windows Remote host** — it registers under your account with a machine ID.
3. Set the access policy per machine: ask for consent every time, always allow, or allow with a reconnect grace period.
4. Open the **macOS viewer** (or the web lobby), sign in — your machines appear with live status.
5. Click a machine → session opens: desktop, files and power actions, all inside one window.

## What's in this repository

- `DDNSProRemote-macOS-<version>.dmg` — macOS viewer installer (Developer ID + notarized)
- `DDNSProRemote-macOS-<version>.zip` — update bundle for the in-app updater
- `visor_macos.json` — signed version manifest (Ed25519) read by the auto-updater
- `visor_macos_appcast.xml` — legacy Sparkle feed for pre-1.1.0 installs
- `*.sha256` — checksums for every binary

[Latest release](https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest)

## FAQ

**Is the traffic encrypted?**
Yes — sessions run over WebRTC with DTLS-SRTP; signaling travels over authenticated TLS. Nothing transits in clear, and consent/policies are enforced host-side.

**Do I need a Dynamic DNS Pro subscription?**
Remote is licensed separately — you can buy it on its own. If you already have an account, it shares your login and machine list.

**What's the difference between the viewer and the host?**
The viewer (this repo) is what *you* run to connect; the host (in `dynamicdnspro-releases`) is what runs on the remote machine.

**Can I connect without an account?**
Yes — ad-hoc sessions work with the remote machine's ID and password, like classic remote-assistance tools.

## Support

- Website & client portal: [dynamicdnspro.com](https://dynamicdnspro.com)
- Remote web lobby: [remote.dynamicdnspro.com](https://remote.dynamicdnspro.com)
- Email: support@it-systems.es

---
<p align="center"><sub>DDNSPro Remote · © MavkSoft / IT-Systems</sub></p>
