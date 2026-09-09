<p align="center">
  <a href="https://bastr.io/zh/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a>
</p>

# Bastrio：在线 SSH、远程桌面、数据库与 Docker 浏览器工作区

[Bastrio（Bastr.io）](https://bastr.io/zh/) 是面向开发者、运维人员和团队的浏览器远程管理工作区。在一个页面中使用 WebSSH 终端、SFTP 文件管理、RDP/VNC 远程桌面、数据库客户端和 Docker 管理工具，通过保存连接、多标签、分屏及共享工作区衔接日常任务，同时使用加密凭据存储与账户安全保护。

[打开工作区](https://bastr.io/workspace/) · [阅读工具选型指南](../articles/README.md) · [访问官网](https://bastr.io/zh/)

[English](../../README.md) · 简体中文 · [繁體中文](README.zh-TW.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Español](README.es.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [Português](README.pt.md) · [العربية](README.ar.md)

## 从连接服务器，到完成一整项工作

连接主机、打开终端、修改配置、查询数据库、查看容器，可以在同一个工作区里连续完成。左侧主机列表帮助你整理资源，顶部标签和分屏让相关会话同时可见，文件、数据库、Docker 与 AI 工具则跟随当前任务展开。

![Bastrio 浏览器工作区：分屏使用在线 SSH 终端与 SFTP 文件管理器](../images/readme/split-workspace.png)

| 界面区域 | 可以完成的工作 |
| --- | --- |
| 主机与会话 | 保存连接、文件夹分组、按连接类型筛选、打开最近会话，使用多标签与分屏布局。 |
| WebSSH 与远程命令 | 使用密码或 SSH 私钥认证，在浏览器中操作终端、调用快捷命令、搜索输出和重新连接；开放时还可使用 WinRM、Telnet 连接类型。 |
| SFTP、FTP、FTPS 文件管理 | 浏览目录、上传下载、新建文件夹、重命名，以及在终端旁编辑支持的文本文件。 |
| RDP、VNC 远程桌面 | 在浏览器中打开远程桌面，使用会话控制、剪贴板和快捷键；目标设备需要提供可达的 RDP 或 VNC 服务。 |
| 数据库客户端 | 连接 PostgreSQL、MySQL/MariaDB、SQL Server、Redis、MongoDB，使用对应引擎的数据浏览、查询、编辑和备份入口。 |
| Docker 可视化管理 | 添加已有 SSH 主机，发现容器、查看资源用量，管理容器、Compose、镜像、卷与网络，并使用应用模板、自定义镜像或受支持的 Compose 配置部署。 |
| 网络路径 | 选择可用的地区代理线路、自定义代理，或通过 SSH 跳板机连接目标资源。 |
| 共享工作区 | 切换个人与团队工作区、邀请成员，并为需要协作的资源授予访问权限。 |
| AI 与 MCP | 在终端或数据库旁使用 AI 助手，也可以让 MCP 客户端访问你授权的资源。 |
| 加密运维手册与云端存储 | 分类整理工作文档，为敏感手册设置独立密码并加密保存，在可用存储空间中管理文件。 |

协议开放情况、Docker 操作、数据库写入、AI 用量和存储额度，以当前账户、工作区权限及目标服务实际支持为准。界面会显示当前会话可用的能力。

## 加密保护与访问控制

Bastrio 将加密存储、账户保护和授权控制放进日常操作流程：

- **连接凭据加密保存：** 已保存的连接密码与私钥使用 AES-256-GCM 静态加密保护。
- **加密传输：** 通过 HTTPS 访问 Bastr.io；远程连接可选用 SSH/SFTP、FTPS 等提供加密传输的协议。
- **账户安全与恢复：** 支持两步验证，请离线保管恢复密钥；重置密码后，可通过恢复流程重新访问加密连接凭据。
- **手册独立加密：** 对敏感笔记启用加密模式、设置独立文档密码，并在编辑器中确认加密与保存。请妥善保管文档密码。
- **AI 授权可控：** MCP API 密钥支持权限范围、有效期和撤销控制；在浏览器中核对敏感操作的授权请求，通过工作区界面管理服务器凭据。

这些保护与目标系统自身的权限、安全设置共同发挥作用。恢复材料和真实凭据应由你妥善保管，不要放入公开文档、截图或 AI 对话。

## 正在寻找这些工具的浏览器替代方案？

如果你正在比较 Termius 替代品、FinalShell 或 Xshell 的网页版工作方式、Navicat 类数据库工具，或者通过 SSH 管理 Docker 的 Portainer 替代方案，可以先按实际任务选择。Bastrio 的适用场景，是在浏览器中把多种远程资源和协作流程放在一起。

| 常见比较对象 | 适合考虑 Bastrio 的需求 | 详细对比 |
| --- | --- | --- |
| Termius、FinalShell、MobaXterm、Xshell、SecureCRT、PuTTY | 希望使用在线 SSH、保存主机、分屏会话和文件工具；依赖桌面脚本或 X11 时需进一步核对。 | [SSH 工具与浏览器工作区](../articles/zh/ssh-tools-browser-workspace.md) |
| WinSCP、FileZilla、Xftp、Cyberduck | 希望在远程会话旁完成 SFTP 或 FTP/FTPS 上传下载与文本编辑。 | [FTP/SFTP 工具与维护流程](../articles/zh/ftp-sftp-tools-browser-workflow.md) |
| Navicat、DBeaver、DataGrip、pgAdmin、Redis Insight、MongoDB Compass | 希望在浏览器中连接数据库，结合引擎、查询、编辑和备份需求选型。 | [远程数据库管理工具对比](../articles/zh/remote-database-tools-comparison.md) |
| Apache Guacamole、TeamViewer、AnyDesk、ToDesk | 需要在浏览器中访问已有 RDP/VNC 服务；远程协助与桌面网关的连接条件需要分别判断。 | [浏览器远程桌面工具对比](../articles/zh/browser-remote-desktop-tools.md) |
| Portainer、Dockge、Docker Desktop | 希望复用 SSH 主机管理远程 Docker 和 Compose；本地容器开发与集群管理需按另外的需求评估。 | [Docker 可视化工具场景对比](../articles/zh/docker-management-tools-by-scenario.md) |
| MCP 与 SSH、数据库、Docker 工具的组合 | 希望让 AI 客户端在限定权限和授权控制下发现、操作远程资源。 | [MCP 远程管理工具对比](../articles/zh/mcp-remote-management-tools.md) |

上表按工作方式比较，具体能力会因产品版本、配置和使用条件而不同。各篇指南也说明了专用工具更适合的任务。

## 开始使用

1. 访问 [bastr.io](https://bastr.io/zh/)。首页开放访客连接时可临时使用；登录后可以保存和整理工作资源。
2. 在快速连接入口选择协议，或在**主机**中添加目标。密码与私钥只在连接表单中填写。
3. 如果目标需要指定网络路径，选择代理或 SSH 跳板机。
4. 打开会话，按任务进入**文件**、数据库面板或 **Docker**，使用布局按钮安排相关会话。
5. 团队协作时切换到正确的工作区，按需共享资源，并开启两步验证、离线保存恢复材料。

访客入口有独立的可用状态和额度。保存主机、团队协作及部分工具需要登录或相应账户权限。

## 通过 SSH 管理 Docker

在工作区打开 **Docker**，选择你有权限访问的 SSH 主机。界面集中展示容器、Compose、镜像、卷、网络和任务进度，可查看容器状态与资源用量，执行支持的启停操作，并通过应用模板、自定义镜像或受支持的 Compose 配置开始部署。

如果目标尚未安装 Docker，可以在支持的 Linux 主机上查看安装方案并确认执行。实际可用性取决于主机条件、账户权限与当前功能开放情况。[Docker 选型指南](../articles/zh/docker-management-tools-by-scenario.md)提供了按场景评估和试用的思路。

## 让 AI 客户端通过 MCP 接入

Bastrio 支持通过 Model Context Protocol（MCP，模型上下文协议）连接 Claude Code、Codex、Cursor、VS Code 等客户端。它与内置 AI 助手配合使用，让你选择的客户端访问经过授权的主机、文件、数据库与网络路径。

1. 在工作区打开**常用工具 → MCP API 密钥**。
2. 根据客户端需要选择权限范围与有效期，创建密钥。
3. 在页面中选择客户端，使用对应的连接说明。
4. 使用客户端支持的密钥或环境变量配置方式保存 API 密钥；在浏览器中核对授权请求，不再使用时撤销访问。

连接地址以账户页面显示为准；可用工具取决于授予的权限，由客户端从 MCP 服务发现。阅读 [MCP 远程管理指南](../articles/zh/mcp-remote-management-tools.md)，了解它与 SSH、数据库、Docker 工作的衔接方式。

## 六篇对比文章，十种语言

[工具选型文库](../articles/README.md)收录六篇已发布文章的英文、简体中文、繁体中文、西班牙语、德语、法语、日语、韩语、马来语和俄语版本。正文沿用已有译文，保留配图、常见问题及对应的 Bastr.io 原文链接。

[简体中文](../articles/zh/README.md) · [English](../articles/en/README.md) · [繁體中文](../articles/zh-TW/README.md) · [日本語](../articles/ja/README.md) · [한국어](../articles/ko/README.md) · [Español](../articles/es/README.md) · [Deutsch](../articles/de/README.md) · [Français](../articles/fr/README.md) · [Bahasa Melayu](../articles/ms/README.md) · [Русский](../articles/ru/README.md)

## 常见问题

### Bastrio 是什么？

Bastrio 是集 WebSSH、文件传输、RDP/VNC、数据库、Docker 管理、共享资源与 AI 辅助于一体的浏览器工作区，适合需要同时处理多种远程系统的开发者和运维人员。

### Bastrio 可以替代 Termius、FinalShell 或 MobaXterm 吗？

对于常见 SSH 会话与文件管理，Bastrio 提供浏览器中的工作方式。迁移前还应核对本地终端集成、宏、X11 等实际依赖，可参考 [SSH 工具对比](../articles/zh/ssh-tools-browser-workspace.md)按场景选择。

### Bastrio 可以作为 Navicat、DBeaver 的网页版替代方案吗？

Bastrio 支持 PostgreSQL、MySQL/MariaDB、SQL Server、Redis 与 MongoDB 的常见远程数据库工作。操作范围随引擎和权限变化；高级建模、同步以及专项开发需求仍需按实际任务评估。

### Bastrio 是 Portainer 的替代方案吗？

如果你需要通过已有 SSH 连接，在终端和数据库旁管理 Docker 主机与 Compose，Bastrio 可以作为浏览器工作方案进行评估。请结合 [Docker 工具对比](../articles/zh/docker-management-tools-by-scenario.md)判断自己的部署需求。

### 使用前需要安装桌面客户端吗？

可以直接在受支持的浏览器中使用工作区。目标仍需提供可达的 SSH、文件传输、远程桌面或数据库服务，并具备有效访问凭据。

### 连接密码与敏感笔记如何保护？

已保存的连接凭据使用 AES-256-GCM 静态加密，浏览器通过 HTTPS 访问 Bastr.io。敏感运维手册可使用独立文档密码加密保存，账户还提供两步验证、恢复材料和资源权限控制。

### 可以免登录使用吗？

首页开放访客连接时可以使用。支持协议、使用时长与可用状态以页面显示为准；保存连接及更多工作区工具需要登录并具备相应权限。

## 联系与项目信息

官网：[bastr.io](https://bastr.io/zh/) · 支持邮箱：[sup@bastr.io](mailto:sup@bastr.io) · [反馈问题](https://github.com/cihalqe/bastrio/issues)

本仓库提供 Bastrio 的公开产品文档与使用指南，欢迎提出建议、纠错或补充使用体验。Issue 和 Pull Request 请使用不含敏感信息的示例。

许可证：[GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html)。
