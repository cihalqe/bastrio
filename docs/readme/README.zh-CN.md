<p align="center"><a href="https://bastr.io/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a></p>

<p align="center">用于安全远程访问、基础设施操作与协同工作的浏览器工作站。</p>

<p align="center"><a href="https://bastr.io/"><strong>bastr.io</strong></a> &nbsp;|&nbsp; <a href="https://www.gnu.org/licenses/gpl-3.0.html"><img src="https://img.shields.io/badge/license-GPL--3.0--only-2b82f0.svg" alt="GPL-3.0-only" /></a></p>

<p align="center"><a href="../../README.md">English</a> | <strong>简体中文</strong> | <a href="README.zh-TW.md">繁體中文</a> | <a href="README.ja.md">日本語</a> | <a href="README.ko.md">한국어</a> | <a href="README.es.md">Español</a> | <a href="README.de.md">Deutsch</a> | <a href="README.fr.md">Français</a> | <a href="README.pt.md">Português</a> | <a href="README.ar.md">العربية</a></p>

## 一个浏览器工作站，覆盖远程基础设施

[Bastrio](https://bastr.io/) 将**在线 SSH**、SFTP、FTP/FTPS、RDP、VNC 与数据库连接集中到一个浏览器工作站。它既是 Web SSH 终端、在线文件管理器和浏览器数据库客户端，也是一套供团队协作管理远程服务器的工作空间。

![Bastrio 在线 SSH 与浏览器远程访问工作站](../images/readme/ssh-online-guest.png)

## 核心能力

- **浏览器直连：** 在线 SSH 终端、SFTP/FTP/FTPS 文件管理，以及 RDP、VNC 远程桌面。
- **统一数据库工具：** 在同一工作区连接 PostgreSQL、MySQL/MariaDB、SQL Server、Redis 与 MongoDB。
- **有序管理连接：** 保存连接、文件夹分组、类型筛选、最近连接、多会话与分屏布局。
- **自己选择网络路径：** 按地区选择代理 IP，配置自定义代理，或通过 SSH 跳板机访问未直接暴露的基础设施。
- **AI 辅助操作：** 在终端和数据库工作旁使用 AI 助手解释输出、编写命令并协助日常操作。
- **协同工作站：** 工作空间与共享资源让团队保留连接上下文并协同处理基础设施事务。
- **加密操作文档：** 在工作空间内编写、加密和保存敏感笔记、草稿与工作文本。

<p align="center"><img src="../images/readme/ssh-online-terminal.png" width="49%" alt="Bastrio 在线 SSH 终端" /> <img src="../images/readme/connection-types.png" width="49%" alt="Bastrio 连接类型" /></p>

<p align="center"><img src="../images/readme/remote-workspace.png" width="49%" alt="Bastrio 远程工作站" /> <img src="../images/readme/sftp-file-browser.png" width="49%" alt="Bastrio SFTP 文件浏览器" /></p>

<p align="center"><img src="../images/readme/proxy-region-picker.png" width="49%" alt="Bastrio 代理地区选择" /> <img src="../images/readme/split-workspace.png" width="49%" alt="Bastrio 分屏工作站" /></p>

<p align="center"><img src="../images/readme/postgresql-workspace.png" width="49%" alt="Bastrio PostgreSQL 工作区" /> <img src="../images/readme/encrypted-operations-documents.png" width="49%" alt="Bastrio 加密操作文档" /></p>

<p align="center"><img src="../images/readme/recovery-key.png" width="49%" alt="Bastrio 恢复密钥" /></p>

## 可控的网络路径

Bastrio 让浏览器远程访问使用适合当前任务的路径：需要出口地区时选择**代理 IP**；需要路径控制时使用自定义代理；需要访问内网或未公开的基础设施时使用 **SSH 跳板机**。这些选择就在连接设置中，无需切换到额外工具。

## 专注且可协同的远程工作

Bastrio 面向需要频繁切换服务器、文件、桌面和数据库的开发者、运维人员与团队。工作空间和共享资源保留上下文，多会话和分屏保持关联任务可见，AI 助手始终贴近终端或数据库工作。

## 隐私设计

凭据和私有工作空间内容在传输中及静态保存时均会加密。Bastrio 只会在已授权操作所需的服务器易失内存中临时解密凭据；明文不会写入磁盘或日志。每一次用户可见的访问都需要有效登录会话。会话过期或被撤销后，均无法再访问或解密加密保险库。恢复密钥仅展示一次；重置密码后需要它来恢复已加密凭据。没有该密钥，加密保险库无法恢复或以可读形式导出。

## Marketplace，计划中

Bastrio 正在规划托管服务器与代理 IP 服务的 Marketplace。它们属于后续版本计划，当前并非已可用服务。

## 开始使用

1. 访问 [bastr.io](https://bastr.io/) 打开 Bastrio 远程工作站。
2. 选择 SSH、文件传输、远程桌面或数据库连接。
3. 需要时选择网络路径，再保存并整理连接以便后续工作。

## 常见问题

### Bastrio 是 Web SSH 终端吗？

是。Bastrio 提供浏览器中的在线 SSH，并将其与文件传输、远程桌面、数据库、代理及工作空间工具放在一起。

### 可以使用代理 IP、自定义代理和 SSH 跳板机吗？

可以。Bastrio 支持按地区选择代理 IP、自定义代理配置以及 SSH 跳板机。

### 团队可以在同一环境中协作吗？

可以。工作空间和共享资源用于让远程基础设施工作保持有序并便于协同。

## 联系方式

邮箱：[sup@bastr.io](mailto:sup@bastr.io)

## 贡献

欢迎提交贡献和问题报告。请保持建议聚焦于用户可见行为，并不要在 issue 或 pull request 中提交凭据或私有连接数据。

## 许可证

Bastrio 使用 [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html) 发布。
