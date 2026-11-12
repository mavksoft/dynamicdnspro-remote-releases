<p align="center">
  <img src="https://dynamicdnspro.com/assets/img/logo.png" alt="Dynamic DNS Pro" width="96">
</p>

<h1 align="center">DDNSPro Remote</h1>

<p align="center">Tus equipos, a un clic.<br>Escritorio remoto WebRTC seguro — visor nativo para macOS, agente remoto para Windows.</p>

<p align="center">
  <a href="https://remote.dynamicdnspro.com"><img src="https://img.shields.io/badge/website-remote.dynamicdnspro.com-0A84FF" alt="website"></a>
  <a href="https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest"><img src="https://img.shields.io/github/v/release/mavksoft/dynamicdnspro-remote-releases?label=latest" alt="latest release"></a>
  <img src="https://img.shields.io/badge/platform-macOS%20%C2%B7%20Windows-black" alt="platforms">
  <img src="https://img.shields.io/badge/license-commercial-orange" alt="commercial license">
</p>

<p align="center"><a href="https://mavksoft.github.io/dynamicdnspro-remote-releases/"><img src="https://img.shields.io/static/v1?label=docs&message=mavksoft.github.io/dynamicdnspro-remote-releases&color=blue" alt="docs"></a></p>

<p align="center">🌍 <strong>🇪🇸 Español</strong> · <a href="README.md">🇬🇧 English</a> · <a href="README.de.md">🇩🇪 Deutsch</a> · <a href="README.fr.md">🇫🇷 Français</a> · <a href="README.it.md">🇮🇹 Italiano</a> · <a href="README.pt.md">🇵🇹 Português</a></p>

> **Este repositorio publica únicamente releases oficiales** — el código fuente es privado. Descargas firmadas, checksums y feeds de auto-actualización.

## Descarga

| | |
|---|---|
| <img src='https://raw.githubusercontent.com/mavksoft/dynamicdnspro-remote-releases/main/icons/apple.svg' width='15' style='vertical-align:-2px' alt='apple'> **Visor (macOS)** | [DDNSProRemote-macOS.dmg](https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest) — cliente nativo, firmado Developer ID y notarizado |
| <img src='https://raw.githubusercontent.com/mavksoft/dynamicdnspro-remote-releases/main/icons/windows.svg' width='15' style='vertical-align:-2px' alt='windows'> **Host remoto (Windows)** | [DynamicDNSPro-Remote-Setup.exe](https://github.com/mavksoft/dynamicdnspro-releases/releases/latest) — instálalo en los equipos a los que quieras acceder |
| <img src='https://dynamicdnspro.com/assets/img/logo.png' width='15' style='vertical-align:-2px'> **Visor web** | [remote.dynamicdnspro.com](https://remote.dynamicdnspro.com) — sesiones completas desde cualquier navegador, sin instalar nada |
| <img src='https://dynamicdnspro.com/assets/img/logo.png' width='15' style='vertical-align:-2px'> **Web oficial** | [dynamicdnspro.com](https://dynamicdnspro.com) — acceso clientes, planes y FAQ |

## Qué es

DDNSPro Remote es el producto de acceso remoto del ecosistema Dynamic DNS Pro — con licencia independiente, pero compartiendo tu cuenta, tus equipos y tus permisos con el portal web. Instala el host en los equipos que administras y accede a ellos desde el visor nativo de macOS o cualquier navegador: escritorio, archivos, consola y acciones de energía sobre WebRTC cifrado de extremo a extremo.

<p align="center"><img src="./screenshots/website.png" width="640" alt="screenshot"></p>

## Funciones

- **Sesiones WebRTC P2P** — vídeo de escritorio, audio e input de baja latencia con cifrado DTLS extremo a extremo.
- **Acceso por consentimiento** — el lado remoto aprueba cada sesión (o defines permiso permanente/de reconexión por equipo).
- **Gestor de archivos** — explora unidades remotas, sube y descarga con arrastrar y soltar dentro de la sesión.
- **Lobby de equipos** — tus máquinas con miniaturas en vivo, o conexiones puntuales por ID + contraseña.
- **Selector de sesión RDP** — en hosts multi-sesión, elige una sesión existente o abre una nueva.
- **Control de resolución** — cambia la resolución remota en caliente (perfiles admin).
- **Espera tras reinicio** — reinicia el equipo remoto y la sesión espera y se reengancha sola.
- **Acciones de energía** — reinicio, bloqueo, Ctrl+Alt+Supr / SAS, Win+D desde la barra de sesión.
- **Portapapeles, cursor remoto, teclado y ratón** — paridad total de input con el visor web.
- **Auto-actualización firmada** — manifiestos Ed25519; las builds de macOS están notarizadas por Apple.
- **Seis idiomas** — ES / EN / FR / IT / DE / PT.

## Cómo se usa

1. Regístrate en [dynamicdnspro.com](https://dynamicdnspro.com) y activa un plan Remote.
2. En cada equipo al que quieras acceder, instala el **host Remote para Windows** — se registra en tu cuenta con un ID de equipo.
3. Define la política de acceso por equipo: pedir consentimiento siempre, permitir siempre, o permitir con periodo de gracia de reconexión.
4. Abre el **visor macOS** (o el lobby web), inicia sesión — tus equipos aparecen con su estado en vivo.
5. Clic en un equipo → se abre la sesión: escritorio, archivos y acciones de energía en una sola ventana.

## Qué contiene este repositorio

- `DDNSProRemote-macOS-<versión>.dmg` — instalador del visor macOS (Developer ID + notarizado)
- `DDNSProRemote-macOS-<versión>.zip` — paquete de actualización para el updater integrado
- `visor_macos.json` — manifiesto de versión firmado (Ed25519) que lee el auto-actualizador
- `visor_macos_appcast.xml` — feed Sparkle heredado para instalaciones anteriores a 1.1.0
- `*.sha256` — checksums de cada binario

[Última release](https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest)

## Preguntas frecuentes

**¿El tráfico va cifrado?**
Sí — las sesiones van por WebRTC con DTLS-SRTP; la señalización viaja por TLS autenticado. Nada transita en claro y el consentimiento/políticas se aplican en el host.

**¿Necesito una suscripción de Dynamic DNS Pro?**
Remote se licencia por separado — puedes comprarlo de forma independiente. Si ya tienes cuenta, comparte tu login y tu lista de equipos.

**¿Diferencia entre visor y host?**
El visor (este repo) es lo que *tú* ejecutas para conectar; el host (en `dynamicdnspro-releases`) es lo que corre en el equipo remoto.

**¿Puedo conectar sin cuenta?**
Sí — las sesiones puntuales funcionan con el ID y la contraseña del equipo remoto, como las herramientas clásicas de asistencia.

## Soporte

- Web y acceso clientes: [dynamicdnspro.com](https://dynamicdnspro.com)
- Lobby web Remote: [remote.dynamicdnspro.com](https://remote.dynamicdnspro.com)
- Email: support@it-systems.es

---
<p align="center"><sub>DDNSPro Remote · © MavkSoft / IT-Systems</sub></p>
