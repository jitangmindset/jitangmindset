<p align="center">
  <a href="https://github.com/hrz76xbg48-pixel/varlune">
    <img src="https://raw.githubusercontent.com/hrz76xbg48-pixel/varlune/main/public/varlune-logo.png" width="128" alt="Varlune logo">
  </a>
</p>

<h1 align="center">hrz76xbg48</h1>

<p align="center"><strong>Desktop developer · creator of Varlune</strong></p>

<p align="center">
  I build local-first Windows software with careful security boundaries,<br>
  reliable data migrations and interfaces designed for everyday use.
</p>

<p align="center">
  <a href="https://github.com/hrz76xbg48-pixel/varlune"><img alt="Varlune repository" src="https://img.shields.io/badge/Varlune-source-111111?style=for-the-badge&logo=github&logoColor=white"></a>
  <a href="https://github.com/hrz76xbg48-pixel/varlune/releases/latest"><img alt="Latest Varlune release" src="https://img.shields.io/github/v/release/hrz76xbg48-pixel/varlune?style=for-the-badge&label=release&color=111111"></a>
  <img alt="Varlune tests" src="https://img.shields.io/badge/tests-71%20passed-111111?style=for-the-badge">
</p>

---

## Varlune — flagship project

[Varlune](https://github.com/hrz76xbg48-pixel/varlune) is my largest project: a local-first password manager built as a complete Windows product rather than a UI prototype.

It combines an Electron desktop application, encrypted local storage, a Chromium browser extension and a C# Native Messaging host. Credentials, payment cards, notes and TOTP secrets stay on the user's computer.

### What is already built

- encrypted vault based on `Argon2id` and `AES-256-GCM`;
- logins, cards, structured notes, categories, favourites and TOTP;
- encrypted backups, validated restore and atomic data migrations;
- Chromium extension for credential and payment-card detection;
- authenticated browser-to-desktop bridge through Native Messaging;
- light, dark, system and custom themes;
- Windows installer and portable release builds;
- **71 passing automated tests** covering storage, crypto, recovery and integrations.

### Architecture priorities

| Priority | Implementation |
|---|---|
| Local data ownership | the vault stays on the user's machine |
| Process isolation | sandboxed renderer and narrow IPC surface |
| Recoverability | atomic writes, backups and rollback-safe migrations |
| Secret handling | browser components never receive the vault directly |
| Product completeness | installer, extension, settings, themes and releases |

**[Explore the source code](https://github.com/hrz76xbg48-pixel/varlune)** · **[Download the latest release](https://github.com/hrz76xbg48-pixel/varlune/releases/latest)**

## Languages

<p>
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-111111?style=for-the-badge&logo=javascript&logoColor=F7DF1E">
  <img alt="C Sharp" src="https://img.shields.io/badge/C%23-111111?style=for-the-badge&logo=dotnet&logoColor=9B72CF">
  <img alt="Python" src="https://img.shields.io/badge/Python-111111?style=for-the-badge&logo=python&logoColor=4B8BBE">
  <img alt="HTML5" src="https://img.shields.io/badge/HTML5-111111?style=for-the-badge&logo=html5&logoColor=E34F26">
  <img alt="CSS3" src="https://img.shields.io/badge/CSS3-111111?style=for-the-badge&logo=css&logoColor=663399">
</p>

## Tools and platforms

<p>
  <img alt="Electron" src="https://img.shields.io/badge/Electron-111111?style=for-the-badge&logo=electron&logoColor=9FEAF9">
  <img alt="Node.js" src="https://img.shields.io/badge/Node.js-111111?style=for-the-badge&logo=nodedotjs&logoColor=5FA04E">
  <img alt="Vite" src="https://img.shields.io/badge/Vite-111111?style=for-the-badge&logo=vite&logoColor=AC6CFF">
  <img alt="Git" src="https://img.shields.io/badge/Git-111111?style=for-the-badge&logo=git&logoColor=F05032">
  <img alt="GitHub" src="https://img.shields.io/badge/GitHub-111111?style=for-the-badge&logo=github&logoColor=white">
  <img alt="Windows" src="https://img.shields.io/badge/Windows-111111?style=for-the-badge&logo=windows11&logoColor=46A2F1">
</p>

## How I build

`define boundaries` → `implement the real flow` → `test failure paths` → `ship an installable result`

I care about predictable behavior, readable interfaces and preserving user data when software is upgraded, restored or interrupted at the wrong moment.

---

<p align="center"><sub>Varlune is actively evolving one verified release at a time.</sub></p>
