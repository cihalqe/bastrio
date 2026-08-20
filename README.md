<p align="center">
  <a href="https://bastr.io/">
    <img src="docs/images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" />
  </a>
</p>

<p align="center">
  A browser workspace for secure remote access, infrastructure work, and collaboration.
</p>

<p align="center">
  <a href="https://bastr.io/"><strong>bastr.io</strong></a>
  &nbsp;|&nbsp;
  <a href="https://www.gnu.org/licenses/gpl-3.0.html"><img src="https://img.shields.io/badge/license-GPL--3.0--only-2b82f0.svg" alt="GPL-3.0-only" /></a>
  <a href="https://github.com/cihalqe/bastrio"><img src="https://img.shields.io/badge/self--hosted-remote%20workspace-0f766e.svg" alt="Self-hosted remote workspace" /></a>
</p>

<p align="center">
  <strong>English</strong> | <a href="docs/readme/README.zh-CN.md">简体中文</a> | <a href="docs/readme/README.zh-TW.md">繁體中文</a> | <a href="docs/readme/README.ja.md">日本語</a> | <a href="docs/readme/README.ko.md">한국어</a> | <a href="docs/readme/README.es.md">Español</a> | <a href="docs/readme/README.de.md">Deutsch</a> | <a href="docs/readme/README.fr.md">Français</a> | <a href="docs/readme/README.pt.md">Português</a> | <a href="docs/readme/README.ar.md">العربية</a>
</p>

## One workspace for remote infrastructure

[Bastrio](https://bastr.io/) brings **SSH online**, SFTP, FTP/FTPS, RDP, VNC, and database connections into a focused browser workspace. Use it as a web SSH terminal, an online file manager, a browser database client, or a shared remote-server management space without switching between separate tools.

![Bastrio SSH online and browser remote access workspace](docs/images/readme/ssh-online-guest.png)

## What you can do

- **Connect from the browser.** Open SSH terminals, manage files through SFTP, FTP, or FTPS, and work with RDP and VNC remote desktops.
- **Work with databases in one place.** Connect to PostgreSQL, MySQL/MariaDB, SQL Server, Redis, and MongoDB alongside your remote hosts.
- **Organize real infrastructure.** Save connections, group them into folders, filter by type, reopen recent sessions, and work across multiple panes.
- **Choose your network path.** Use platform proxy IP routes by region, bring a custom proxy, or reach private infrastructure through an SSH jump host.
- **Keep momentum with AI.** Use the AI assistant beside terminal and database work to explain output, draft commands, and help with day-to-day operations.
- **Collaborate in workspaces.** Share the resources your team needs, keep connection context organized, and use the same workspace across operational tasks.
- **Protect sensitive notes.** Create encrypted operations documents for passwords, drafts, and private working text inside the workspace.

## Remote access without tool sprawl

| Connect | Manage | Organize |
| --- | --- | --- |
| SSH online and web SSH terminal | SFTP, FTP, and FTPS files | Folders, filters, and recent connections |
| RDP and VNC desktop sessions | PostgreSQL, MySQL/MariaDB, SQL Server, Redis, MongoDB | Multiple sessions and split layouts |

<p align="center">
  <img src="docs/images/readme/ssh-online-terminal.png" width="49%" alt="Bastrio online SSH terminal" />
  <img src="docs/images/readme/connection-types.png" width="49%" alt="Bastrio connection type picker" />
</p>

<p align="center">
  <img src="docs/images/readme/remote-workspace.png" width="49%" alt="Bastrio remote workspace" />
  <img src="docs/images/readme/sftp-file-browser.png" width="49%" alt="Bastrio SFTP file browser" />
</p>

<p align="center">
  <img src="docs/images/readme/proxy-region-picker.png" width="49%" alt="Bastrio proxy region picker" />
  <img src="docs/images/readme/split-workspace.png" width="49%" alt="Bastrio split SSH and file workspace" />
</p>

<p align="center">
  <img src="docs/images/readme/postgresql-workspace.png" width="49%" alt="Bastrio PostgreSQL workspace" />
  <img src="docs/images/readme/encrypted-operations-documents.png" width="49%" alt="Bastrio encrypted operations documents" />
</p>

<p align="center">
  <img src="docs/images/readme/recovery-key.png" width="49%" alt="Bastrio recovery key" />
</p>

## Network paths you control

Bastrio supports browser remote access through the route that fits the job. Select a regional **proxy IP** when you need an egress location, configure your own proxy when you need control of the path, or use an **SSH jump host** to reach infrastructure that is not directly exposed. These options sit next to connection setup instead of becoming a separate workflow.

## Built for focused, collaborative work

Bastrio is a remote workspace for developers, operators, and teams that need to move between servers, files, desktops, and databases quickly. Workspaces and shared resources preserve context; multi-session and split layouts keep related work visible; the AI assistant remains close to the terminal or database task where it is useful.

## Privacy by design

Credentials and private workspace content are encrypted in transit and at rest. Bastrio decrypts credentials only temporarily in volatile server memory when an authorized operation requires them; plaintext is never written to disk or logs. Every user-visible access requires a valid authenticated session. Once a session expires or is revoked, the encrypted vault can no longer be accessed or decrypted. The recovery key is shown only once; it is required to restore encrypted credentials after a password reset. Without it, the encrypted vault cannot be recovered or exported in readable form.

## Marketplace, planned

Bastrio is preparing a Marketplace for managed servers and proxy IP services. These offerings are planned for a future release; this README does not represent them as currently available.

## Get started

1. Visit [bastr.io](https://bastr.io/) to open the Bastrio remote workspace.
2. Choose SSH, file transfer, remote desktop, or a database connection.
3. Select a network path when needed, then save and organize the connection for later work.

## FAQ

### Is Bastrio a web SSH terminal?

Yes. Bastrio provides SSH online in a browser and places it beside file transfer, remote desktop, database, proxy, and workspace tools.

### Which remote protocols and databases are supported?

SSH, SFTP, FTP, FTPS, RDP, VNC, PostgreSQL, MySQL/MariaDB, SQL Server, Redis, and MongoDB are available from the same browser remote-access workspace.

### Can I use a proxy IP, custom proxy, or SSH jump host?

Yes. Bastrio supports regional proxy IP selection, custom proxy configuration, and SSH jump hosts for the connection path you need.

### Can teams work from the same environment?

Yes. Workspaces and shared resources are designed to keep remote infrastructure work organized and collaborative.

## Contact

Email: [sup@bastr.io](mailto:sup@bastr.io)

## Contributing

Contributions and issue reports are welcome. Please keep proposals focused, document user-visible behavior, and avoid adding credentials or private connection data to issues or pull requests.

## License

Bastrio is released under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).
