<p align="center"><a href="https://bastr.io/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a></p>

<p align="center">用於安全遠端存取、基礎設施操作與協同工作的瀏覽器工作站。</p>

<p align="center"><a href="https://bastr.io/"><strong>bastr.io</strong></a> &nbsp;|&nbsp; <a href="https://www.gnu.org/licenses/gpl-3.0.html"><img src="https://img.shields.io/badge/license-GPL--3.0--only-2b82f0.svg" alt="GPL-3.0-only" /></a></p>

<p align="center"><a href="../../README.md">English</a> | <a href="README.zh-CN.md">简体中文</a> | <strong>繁體中文</strong> | <a href="README.ja.md">日本語</a> | <a href="README.ko.md">한국어</a> | <a href="README.es.md">Español</a> | <a href="README.de.md">Deutsch</a> | <a href="README.fr.md">Français</a> | <a href="README.pt.md">Português</a> | <a href="README.ar.md">العربية</a></p>

## 一個瀏覽器工作站，涵蓋遠端基礎設施

[Bastrio](https://bastr.io/) 將**線上 SSH**、SFTP、FTP/FTPS、RDP、VNC 與資料庫連線集中到一個瀏覽器工作站。它同時是 Web SSH 終端機、線上檔案管理器與瀏覽器資料庫用戶端，也是讓團隊協同管理遠端伺服器的工作空間。

![Bastrio 線上 SSH 與瀏覽器遠端存取工作站](../images/readme/ssh-online-guest.png)

## 核心能力

- **瀏覽器連線：** 線上 SSH 終端機、SFTP/FTP/FTPS 檔案管理，以及 RDP、VNC 遠端桌面。
- **整合資料庫工具：** 在同一工作區連線 PostgreSQL、MySQL/MariaDB、SQL Server、Redis 與 MongoDB。
- **有序管理連線：** 儲存連線、資料夾分類、類型篩選、最近連線、多工作階段與分割版面。
- **自行選擇網路路徑：** 依地區選擇代理 IP、設定自訂代理，或透過 SSH 跳板機存取未直接公開的基礎設施。
- **AI 輔助操作：** 讓 AI 助手在終端機與資料庫工作旁協助解讀輸出、撰寫命令與日常操作。
- **協同工作站：** 工作空間與共享資源使團隊能保留連線脈絡並協同處理工作。
- **加密操作文件：** 在工作空間內撰寫、加密與保存敏感筆記、草稿和工作文字。

<p align="center"><img src="../images/readme/ssh-online-terminal.png" width="49%" alt="Bastrio 線上 SSH 終端機" /> <img src="../images/readme/connection-types.png" width="49%" alt="Bastrio 連線類型" /></p>

<p align="center"><img src="../images/readme/remote-workspace.png" width="49%" alt="Bastrio 遠端工作站" /> <img src="../images/readme/sftp-file-browser.png" width="49%" alt="Bastrio SFTP 檔案瀏覽器" /></p>

<p align="center"><img src="../images/readme/proxy-region-picker.png" width="49%" alt="Bastrio 代理地區選擇" /> <img src="../images/readme/split-workspace.png" width="49%" alt="Bastrio 分割工作站" /></p>

<p align="center"><img src="../images/readme/postgresql-workspace.png" width="49%" alt="Bastrio PostgreSQL 工作區" /> <img src="../images/readme/encrypted-operations-documents.png" width="49%" alt="Bastrio 加密操作文件" /></p>

<p align="center"><img src="../images/readme/recovery-key.png" width="49%" alt="Bastrio 復原金鑰" /></p>

## 可控的網路路徑

Bastrio 讓瀏覽器遠端存取採用符合工作需求的路徑：需要出口地區時選擇**代理 IP**；需要控制路徑時使用自訂代理；需要存取內網或未公開基礎設施時使用 **SSH 跳板機**。這些設定都在連線流程內，無須切換工具。

## 專注且可協同的遠端工作

Bastrio 面向需在伺服器、檔案、桌面與資料庫間頻繁切換的開發者、維運人員與團隊。工作空間和共享資源保留脈絡，多工作階段和分割版面維持相關工作可見，AI 助手則貼近終端機或資料庫任務。

## 隱私設計

憑據和私有工作空間內容在傳輸中與靜態保存時均會加密。Bastrio 僅在已授權操作所需的伺服器易失性記憶體中暫時解密憑據；明文不會寫入磁碟或日誌。每次使用者可見存取都需要有效登入工作階段。工作階段到期或遭撤銷後，加密保存庫即無法再被存取或解密。恢復金鑰只顯示一次；重設密碼後需要它才能恢復已加密憑據。沒有該金鑰，加密保存庫無法復原或以可讀形式匯出。

## Marketplace，規劃中

Bastrio 正在規劃託管伺服器與代理 IP 服務的 Marketplace。它們屬於後續版本計畫，目前並非已可用服務。

## 開始使用

1. 前往 [bastr.io](https://bastr.io/) 開啟 Bastrio 遠端工作站。
2. 選擇 SSH、檔案傳輸、遠端桌面或資料庫連線。
3. 需要時選擇網路路徑，再儲存並整理連線供後續工作使用。

## 常見問題

### Bastrio 是 Web SSH 終端機嗎？

是。Bastrio 提供瀏覽器中的線上 SSH，並將檔案傳輸、遠端桌面、資料庫、代理和工作空間工具整合在一起。

### 可以使用代理 IP、自訂代理與 SSH 跳板機嗎？

可以。Bastrio 支援依地區選擇代理 IP、自訂代理設定與 SSH 跳板機。

### 團隊可以在相同環境中協同嗎？

可以。工作空間和共享資源讓遠端基礎設施工作保持有序並利於協同。

## 貢獻

歡迎提交貢獻和問題回報。請讓提案聚焦於使用者可見行為，並勿在 issue 或 pull request 中提交憑據或私有連線資料。

## 授權條款

Bastrio 以 [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html) 發布。
