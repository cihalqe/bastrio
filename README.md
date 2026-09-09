<p align="center">
  <a href="https://bastr.io/en/"><img src="docs/images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a>
</p>

# Bastrio — WebSSH, remote desktops, databases and Docker in your browser

[Bastrio (Bastr.io)](https://bastr.io/en/) is a browser workspace for remote server management. Open an online SSH terminal, transfer files over SFTP, connect to RDP or VNC desktops, work with databases, and manage Docker hosts in one place. Saved connections, split views, shared workspaces and AI assistance keep related tasks together, with encrypted credential storage and account protection built into the workflow.

[Open workspace](https://bastr.io/workspace/) · [Read the guides](docs/articles/README.md) · [Website](https://bastr.io/en/)

English · [简体中文](docs/readme/README.zh-CN.md) · [繁體中文](docs/readme/README.zh-TW.md) · [日本語](docs/readme/README.ja.md) · [한국어](docs/readme/README.ko.md) · [Español](docs/readme/README.es.md) · [Deutsch](docs/readme/README.de.md) · [Français](docs/readme/README.fr.md) · [Português](docs/readme/README.pt.md) · [العربية](docs/readme/README.ar.md)

## A workspace that follows the task

Start with a host, open its terminal, inspect a configuration file, check the database and review a container without rebuilding your connection context in several applications. Bastrio brings the tools next to the work: a host sidebar, session tabs, split layouts, file and database panels, and dedicated Docker and AI views.

![Bastrio browser workspace with SSH terminal and SFTP file manager in a split layout](docs/images/readme/split-workspace.png)

| Area | What you can do from the UI |
| --- | --- |
| Hosts and sessions | Save connections, organize folders, filter connection types, reopen recent sessions, and arrange tabs or split views. |
| WebSSH and remote commands | Use SSH password or private-key authentication, a browser terminal, quick commands, search and reconnect controls. WinRM and Telnet connection types are also available where enabled. |
| SFTP, FTP and FTPS | Browse directories, upload and download files, create folders, rename files, and edit supported text files beside a terminal. |
| RDP and VNC | Open remote desktops in the browser, with session controls, clipboard tools and keyboard shortcuts. The target needs an accessible RDP or VNC service. |
| Database client | Connect to PostgreSQL, MySQL/MariaDB, SQL Server, Redis and MongoDB. Use the engine's data browser and available query, editing and backup tools. |
| Docker | Add an existing SSH host, discover containers, view resource usage, and work with containers, Compose projects, images, volumes and networks. Use application templates or supported custom image and Compose workflows. |
| Network paths | Choose an available regional proxy route, configure your own proxy, or use an SSH jump host. |
| Shared workspaces | Switch between personal and team workspaces, invite members, and grant access to selected resources. |
| AI and MCP | Ask for help beside terminal or database work, or connect an MCP client to the resources you authorize. |
| Encrypted Runbooks and Cloud Storage | Organize working documents, encrypt sensitive runbooks with a separate password, and manage files in your available storage. |

Available protocols, Docker actions, database writes, AI usage and storage depend on your account, workspace permissions and the connected service. The current interface shows what is available for your session.

## Encryption and access you control

Bastrio combines encrypted storage with visible account and connection controls:

- **Encrypted connection credentials.** Saved connection passwords and private keys are protected at rest with AES-256-GCM.
- **Protected transport.** Use Bastr.io over HTTPS. SSH/SFTP and FTPS provide encrypted remote transport; choose a secure protocol appropriate to the destination.
- **Account protection.** Enable two-factor authentication and keep your recovery key offline. The recovery workflow helps restore access to encrypted connection credentials after a password reset.
- **Encrypted runbooks.** Choose encrypted mode and a separate document password for sensitive notes. Confirm encryption and saving in the editor, and keep the document password safe.
- **Controlled AI access.** MCP API keys have selected permissions, expiry and revocation controls. Review browser approval requests before allowing sensitive operations, and manage server credentials through the workspace UI.

These protections work together with the permissions and security of your remote systems. Keep recovery material and real credentials out of shared documents, screenshots and AI conversations.

## WebSSH, database and Docker tool alternatives

Bastrio is useful when your main requirement is a shared browser workflow across several kinds of remote resource. If you are comparing a Termius alternative, a browser alternative to FinalShell or Xshell, a Navicat-style database client, or a Portainer alternative for Docker over SSH, start with the task you need to complete.

| Tools you may be comparing | When to consider Bastrio | Detailed guide |
| --- | --- | --- |
| Termius, FinalShell, MobaXterm, Xshell, SecureCRT and PuTTY | You want browser SSH, saved hosts, split sessions and nearby file tools. Check any desktop scripting or X11 requirements separately. | [SSH tools and browser workspaces](docs/articles/en/ssh-tools-browser-workspace.md) |
| WinSCP, FileZilla, Xftp and Cyberduck | You want SFTP or FTP/FTPS transfers and text editing alongside your remote session. | [FTP/SFTP tools and workflow](docs/articles/en/ftp-sftp-tools-browser-workflow.md) |
| Navicat, DBeaver, DataGrip, pgAdmin, Redis Insight and MongoDB Compass | You want a browser database client next to your hosts. Choose by engine, query, editing and backup needs. | [Remote database tools](docs/articles/en/remote-database-tools-comparison.md) |
| Apache Guacamole, TeamViewer, AnyDesk and ToDesk | You need browser access to an existing RDP/VNC destination. Attended remote assistance and desktop gateways have different connection requirements. | [Browser remote desktops](docs/articles/en/browser-remote-desktop-tools.md) |
| Portainer, Dockge and Docker Desktop | You want to manage remote Docker and Compose resources through an existing SSH host. Local container development and cluster administration are separate selection criteria. | [Docker management by scenario](docs/articles/en/docker-management-tools-by-scenario.md) |
| MCP workflows alongside SSH, database and Docker tools | You want an AI client to discover and operate authorized resources with permissions and approval controls. | [MCP remote management](docs/articles/en/mcp-remote-management-tools.md) |

These are workflow comparisons. Feature coverage varies by product, edition and configuration; the linked guides explain where a specialist tool may fit better.

## Get started in the browser

1. Visit [bastr.io](https://bastr.io/en/). Use an available guest connection for a temporary session, or sign in to save and organize your work.
2. Choose a connection type and enter the destination in **Quick Connect** or add it under **Hosts**. Enter passwords and private keys only in the connection form.
3. Select a proxy or SSH jump host if the destination needs a specific network path.
4. Open the session. Use **Files**, the database panel or **Docker** for the next task, and arrange related sessions with the layout controls.
5. For team work, select the right workspace and share the resources members need. Enable two-factor authentication and save recovery material before relying on the account for daily access.

Guest access has its own availability and allowance. Saved hosts, team features and some tools require sign-in or an eligible account.

## Docker management over SSH

Open **Docker** in the workspace and select an SSH host you can access. The Docker view brings containers, Compose, images, volumes, networks and task progress together. You can inspect container state and resource use, perform supported lifecycle actions, and start a deployment from the available application templates, a custom image or a supported Compose configuration.

If Docker is missing, the interface can guide installation on supported Linux hosts after you review and confirm the proposed action. Availability depends on the host, your permissions and the current feature access. See the [Docker comparison guide](docs/articles/en/docker-management-tools-by-scenario.md) for a practical evaluation workflow.

## Connect AI clients through MCP

Bastrio supports Model Context Protocol (MCP) connections from clients such as Claude Code, Codex, Cursor and VS Code. MCP complements the built-in AI assistant: it lets your chosen client work with authorized hosts, files, databases and network paths.

1. Open **Tools → MCP API Keys** in the workspace.
2. Create a key with the permissions and expiry your client needs.
3. Select the client and use the connection instructions shown on that page.
4. Keep the key in the client's supported secret or environment configuration. Review approval requests in the browser and revoke access when it is no longer needed.

Use the endpoint shown in your account. Available tools depend on the granted permissions; the client should discover them from the MCP service. Read the [MCP guide](docs/articles/en/mcp-remote-management-tools.md) for examples of how this fits with SSH, database and Docker work.

## Six practical guides, ten languages

The [guide library](docs/articles/README.md) contains the six published comparisons in English, Simplified Chinese, Traditional Chinese, Spanish, German, French, Japanese, Korean, Malay and Russian. Each version keeps the existing article text, illustrations, FAQ and a link to its original Bastr.io page.

[English guides](docs/articles/en/README.md) · [简体中文指南](docs/articles/zh/README.md) · [繁體中文指南](docs/articles/zh-TW/README.md) · [日本語](docs/articles/ja/README.md) · [한국어](docs/articles/ko/README.md) · [Español](docs/articles/es/README.md) · [Deutsch](docs/articles/de/README.md) · [Français](docs/articles/fr/README.md) · [Bahasa Melayu](docs/articles/ms/README.md) · [Русский](docs/articles/ru/README.md)

## Frequently asked questions

### What is Bastrio?

Bastrio is a browser workspace that combines WebSSH, file transfer, RDP/VNC, databases, Docker management, shared resources and AI assistance. It is designed for developers and operators who work across several remote systems.

### Can Bastrio replace Termius, FinalShell or MobaXterm?

Bastrio provides a browser workflow for common SSH and file-management tasks. Evaluate the desktop features you rely on, such as local shell integration, macros or X11, before changing tools. The [SSH comparison](docs/articles/en/ssh-tools-browser-workspace.md) helps you choose by scenario.

### Is Bastrio a browser alternative to Navicat or DBeaver?

It can serve common remote database workflows for PostgreSQL, MySQL/MariaDB, SQL Server, Redis and MongoDB. Available operations vary by engine and permissions. Advanced modeling, synchronization and specialized development workflows should be evaluated against your requirements.

### Is Bastrio a Portainer alternative?

For users who want Docker host and Compose management beside SSH, files and databases, Bastrio offers a browser workflow over an existing SSH connection. Compare the [Docker guide](docs/articles/en/docker-management-tools-by-scenario.md) with your environment and deployment needs.

### Do I need to install a desktop client?

You can use the workspace from a supported browser. The target still needs a reachable SSH, file-transfer, remote-desktop or database service and valid access credentials.

### How are connection credentials and sensitive notes protected?

Saved connection credentials use AES-256-GCM encryption at rest, and Bastr.io uses HTTPS for browser access. Sensitive runbooks support encrypted saving with a separate document password. Two-factor authentication, recovery material and resource permissions provide additional controls.

### Can I start without an account?

Use a guest connection when the homepage offers it. Guest access, protocols and time allowances can change; sign in for saved connections and the tools available to your account.

## Contact and project information

Website: [bastr.io](https://bastr.io/en/) · Support: [sup@bastr.io](mailto:sup@bastr.io) · [Report an issue](https://github.com/cihalqe/bastrio/issues)

This repository contains Bastrio's public product documentation and guides. Suggestions and corrections are welcome. Share only non-sensitive examples in issues and pull requests.

License: [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).
