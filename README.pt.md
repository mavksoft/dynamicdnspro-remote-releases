<p align="center">
  <img src="https://dynamicdnspro.com/assets/img/logo.png" alt="Dynamic DNS Pro" width="96">
</p>

<h1 align="center">DDNSPro Remote</h1>

<p align="center">As suas máquinas, a um clique.<br>Ambiente de trabalho remoto WebRTC seguro — visualizador nativo para macOS, host remoto para Windows.</p>

<p align="center">
  <a href="https://remote.dynamicdnspro.com"><img src="https://img.shields.io/badge/website-remote.dynamicdnspro.com-0A84FF" alt="website"></a>
  <a href="https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest"><img src="https://img.shields.io/github/v/release/mavksoft/dynamicdnspro-remote-releases?label=latest" alt="latest release"></a>
  <img src="https://img.shields.io/badge/platform-macOS%20%C2%B7%20Windows-black" alt="platforms">
  <img src="https://img.shields.io/badge/license-commercial-orange" alt="commercial license">
</p>

<p align="center"><a href="https://mavksoft.github.io/dynamicdnspro-remote-releases/"><img src="https://img.shields.io/static/v1?label=docs&message=mavksoft.github.io/dynamicdnspro-remote-releases&color=blue" alt="docs"></a></p>

<p align="center">🌍 <a href="README.es.md">🇪🇸 Español</a> · <a href="README.md">🇬🇧 English</a> · <a href="README.de.md">🇩🇪 Deutsch</a> · <a href="README.fr.md">🇫🇷 Français</a> · <a href="README.it.md">🇮🇹 Italiano</a> · <strong>🇵🇹 Português</strong></p>

> **Este repositório publica apenas releases binárias oficiais** — o código-fonte é privado. Downloads assinados, checksums e feeds de auto-atualização.

## Download

| | |
|---|---|
| <img src='https://raw.githubusercontent.com/mavksoft/dynamicdnspro-remote-releases/main/icons/apple.svg' width='15' style='vertical-align:-2px' alt='apple'> **Visualizador (macOS)** | [DDNSProRemote-macOS.dmg](https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest) — cliente nativo, assinado Developer ID e notarizado |
| <img src='https://raw.githubusercontent.com/mavksoft/dynamicdnspro-remote-releases/main/icons/windows.svg' width='15' style='vertical-align:-2px' alt='windows'> **Host remoto (Windows)** | [DynamicDNSPro-Remote-Setup.exe](https://github.com/mavksoft/dynamicdnspro-releases/releases/latest) — instalar nas máquinas a que quer aceder |
| <img src='https://dynamicdnspro.com/assets/img/logo.png' width='15' style='vertical-align:-2px'> **Visualizador web** | [remote.dynamicdnspro.com](https://remote.dynamicdnspro.com) — sessões completas de qualquer navegador, sem instalação |
| <img src='https://dynamicdnspro.com/assets/img/logo.png' width='15' style='vertical-align:-2px'> **Site oficial** | [dynamicdnspro.com](https://dynamicdnspro.com) — portal de clientes, planos e FAQ |

## O que é

O DDNSPro Remote é o produto de acesso remoto do ecossistema Dynamic DNS Pro — com licença separada, mas partilhando a sua conta, máquinas e permissões com o portal web. Instale o host nas máquinas que administra e aceda-lhes a partir do visualizador macOS nativo ou de qualquer navegador: ambiente de trabalho, ficheiros, consola e ações de energia sobre WebRTC cifrado de ponta a ponta.

<p align="center"><img src="./screenshots/website.png" width="640" alt="screenshot"></p>

## Funcionalidades

- **Sessões WebRTC P2P** — vídeo de ambiente de trabalho, áudio e input de baixa latência com cifragem DTLS ponta a ponta.
- **Acesso por consentimento** — o lado remoto aprova cada sessão (ou permissão permanente/de reconexão por máquina).
- **Gestor de ficheiros** — navegue nas unidades remotas, envios e downloads com arrastar e largar dentro da sessão.
- **Lobby de máquinas** — as suas máquinas com miniaturas ao vivo, ou ligações pontuais por ID + palavra-passe.
- **Seletor de sessão RDP** — em hosts multi-sessão, escolha uma sessão existente ou abra uma nova.
- **Controlo de resolução** — mude a resolução remota a quente (perfis admin).
- **Espera de reconexão** — reinicie a máquina remota: a sessão espera e volta a ligar-se sozinha.
- **Ações de energia** — reinício, bloqueio, Ctrl+Alt+Del / SAS, Win+D na barra de sessão.
- **Área de transferência, cursor remoto, teclado e rato** — paridade total com o visualizador web.
- **Auto-atualizações assinadas** — manifestos Ed25519; builds macOS notarizadas pela Apple.
- **Seis idiomas** — ES / EN / FR / IT / DE / PT.

## Como usar

1. Registe-se em [dynamicdnspro.com](https://dynamicdnspro.com) e ative um plano Remote.
2. Em cada máquina a alcançar, instale o **host Remote para Windows** — regista-se na sua conta com um ID de máquina.
3. Defina a política de acesso por máquina: pedir consentimento sempre, permitir sempre, ou permitir com período de tolerância de reconexão.
4. Abra o **visualizador macOS** (ou o lobby web), inicie sessão — as suas máquinas aparecem com estado ao vivo.
5. Clique numa máquina → a sessão abre: ambiente de trabalho, ficheiros e ações de energia numa só janela.

## Conteúdo deste repositório

- `DDNSProRemote-macOS-<versão>.dmg` — instalador do visualizador macOS (Developer ID + notarizado)
- `DDNSProRemote-macOS-<versão>.zip` — pacote de atualização para o updater integrado
- `visor_macos.json` — manifesto de versão assinado (Ed25519) lido pelo auto-updater
- `visor_macos_appcast.xml` — feed Sparkle herdado para instalações anteriores à 1.1.0
- `*.sha256` — checksums de cada binário

[Última release](https://github.com/mavksoft/dynamicdnspro-remote-releases/releases/latest)

## Perguntas frequentes

**O tráfego é cifrado?**
Sim — as sessões correm sobre WebRTC com DTLS-SRTP; a sinalização viaja por TLS autenticado. Nada transita em claro e o consentimento/políticas são aplicados no host.

**Preciso de uma subscrição do Dynamic DNS Pro?**
O Remote é licenciado à parte — pode comprá-lo isoladamente. Se já tem conta, partilha o seu login e a lista de máquinas.

**Diferença entre visualizador e host?**
O visualizador (este repo) é o que *você* executa para se ligar; o host (em `dynamicdnspro-releases`) corre na máquina remota.

**Posso ligar sem conta?**
Sim — sessões pontuais funcionam com o ID e a palavra-passe da máquina remota, como as ferramentas clássicas de assistência.

## Suporte

- Site e portal de clientes: [dynamicdnspro.com](https://dynamicdnspro.com)
- Lobby web Remote: [remote.dynamicdnspro.com](https://remote.dynamicdnspro.com)
- Email: support@it-systems.es

---
<p align="center"><sub>DDNSPro Remote · © MavkSoft / IT-Systems</sub></p>
