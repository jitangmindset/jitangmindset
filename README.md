<h1 align="center">hrz76xbg48</h1>

<p align="center"><strong>Desktop software · security-minded engineering · Minecraft infrastructure</strong></p>

<p align="center">
  Windows applications that protect local data<br>
  and server tools that fail safely when something goes wrong.
</p>

<p align="center">
  <a href="https://github.com/hrz76xbg48-pixel/varlune">Varlune</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/hrz76xbg48-pixel/paper-server-manager">Paper Server Manager</a>
</p>

---

I build software around the parts that are easy to underestimate: encrypted storage, migrations, backups, browser-to-desktop bridges, verified downloads, rollback behavior and clear failure states.

## Selected work

### 01 — [Varlune](https://github.com/hrz76xbg48-pixel/varlune)

Local-first password manager for Windows. The vault stays on the user's computer while a Chromium extension communicates with the desktop application through a C# Native Messaging host.

`Electron` · `Node.js` · `C#` · `AES-256-GCM` · `Argon2id` · `Native Messaging`

- encrypted credentials, cards, notes and TOTP secrets;
- atomic backups, restore validation and legacy vault migrations;
- sandboxed renderer with narrow IPC boundaries;
- installable Windows releases;
- **71 automated tests passing** across crypto, storage, recovery and browser integration.

[Source code](https://github.com/hrz76xbg48-pixel/varlune) · [Windows releases](https://github.com/hrz76xbg48-pixel/varlune/releases/latest)

### 02 — [Paper Server Manager](https://github.com/hrz76xbg48-pixel/paper-server-manager)

Command-line installer, updater and integrity checker for Paper Minecraft servers. It resolves builds through PaperMC's official downloads API and promotes a download only after its advertised size and SHA-256 digest match.

`Python 3.11+` · `PaperMC API` · `atomic filesystem operations` · `zero runtime dependencies`

- safe install and update commands with stable exit codes;
- server configuration and startup scripts preserved during updates;
- previous JAR retained for rollback;
- clean failure recovery after network or manifest errors;
- **18 automated scenarios passing**, including full CLI install, verify and update flows.

[Source code and usage](https://github.com/hrz76xbg48-pixel/paper-server-manager)

## Verification

| Project | Verified path | Result |
|---|---|---|
| Varlune | syntax checks and complete Node test suite | **71 / 71 passed** |
| Paper Server Manager | unit, integration and CLI end-to-end suite | **18 / 18 passed** |
| Paper Server Manager | official Paper build download | size and SHA-256 matched |

## Engineering focus

| Area | Tools and concerns |
|---|---|
| Desktop | Electron, Node.js, Vite, installers, updates |
| Windows | C#, Native Messaging, system integration |
| Automation | Python, REST APIs, CLI design, structured reports |
| Security | local-first storage, Argon2id, AES-GCM, trust boundaries |
| Game infrastructure | Paper, Velocity, plugin configs, deployment diagnostics |

## How I work

`scope` → `build` → `break intentionally` → `verify recovery` → `ship`

- define the result and trust boundaries before implementation;
- preserve user data and make destructive actions explicit;
- test failure paths, not only the happy path;
- leave the project installable, documented and reproducible.

---

<p align="center"><sub>Build the real path. Verify the failure path. Ship the result.</sub></p>
