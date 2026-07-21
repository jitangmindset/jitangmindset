# hrz76xbg48

I build Windows desktop software, local-first tools and integrations where reliability matters more than decoration.

## Current projects

### [Varlune](https://github.com/hrz76xbg48-pixel/varlune)

A local-first password manager for Windows with an encrypted vault, TOTP, backups, a Chromium extension and a C# Native Messaging host.

The repository includes an installable Windows release and automated tests for the vault format, migrations, backups, browser integration and security boundaries.

### [Paper Server Manager](https://github.com/hrz76xbg48-pixel/paper-server-manager)

A working command-line installer, updater and integrity checker for Paper Minecraft servers. It resolves builds from PaperMC's official API, verifies size and SHA-256 before installation, preserves configuration during updates and keeps a rollback JAR.

The project has no third-party runtime dependencies and includes end-to-end tests for installation, verification, update failure and rollback behavior.

## Areas of work

- Electron and Node.js desktop applications
- C# and Windows integrations
- Python automation and server tooling
- Minecraft Paper and Velocity infrastructure
- application security and local data protection

## Principles

- ship installable software, not screenshots;
- keep trust boundaries explicit;
- make destructive operations deliberate and recoverable;
- verify the real user path from installation to result.
