<p align="center">
  <a href="https://bastr.io/zh-TW/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a>
</p>

# Bastrio：在瀏覽器中使用 WebSSH、遠端桌面、資料庫與 Docker

[Bastrio（Bastr.io）](https://bastr.io/zh-TW/) 是用於管理遠端伺服器的瀏覽器工作區。你可以在同一個地方開啟線上 SSH 終端機、透過 SFTP 傳輸檔案、連線至 RDP 或 VNC 遠端桌面、操作資料庫，以及管理 Docker 主機。已儲存的連線、分割畫面、共享工作區與 AI 輔助讓相關工作保持連貫，連線認證資訊的加密儲存與帳戶保護也整合在日常操作流程中。

[開啟工作區](https://bastr.io/workspace/) · [閱讀指南](../articles/README.md) · [官方網站](https://bastr.io/zh-TW/)

[English](../../README.md) · [简体中文](README.zh-CN.md) · 繁體中文 · [日本語](README.ja.md) · [한국어](README.ko.md) · [Español](README.es.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [Português](README.pt.md) · [العربية](README.ar.md)

## 隨著任務展開的工作區

從連線主機開始，開啟終端機、檢查設定檔、查詢資料庫，再查看容器，都可以在同一個工作區中接續完成。Bastrio 將工具放在工作旁邊：主機側邊欄、工作階段分頁、分割版面、檔案與資料庫面板，以及專用的 Docker 和 AI 檢視，讓你在切換任務時保留連線脈絡。

![Bastrio 瀏覽器工作區：以分割版面並排使用 SSH 終端機與 SFTP 檔案管理器](../images/readme/split-workspace.png)

| 功能區域 | 可在介面中完成的工作 |
| --- | --- |
| 主機與工作階段 | 儲存連線、以資料夾分類、依連線類型篩選、重新開啟最近的工作階段，以及安排分頁或分割畫面。 |
| WebSSH 與遠端命令 | 使用 SSH 密碼或私鑰驗證、瀏覽器終端機、快捷命令、搜尋及重新連線功能。開放時也可使用 WinRM 和 Telnet 連線類型。 |
| SFTP、FTP 與 FTPS | 瀏覽目錄、上傳下載檔案、建立資料夾、重新命名檔案，以及在終端機旁編輯支援的文字檔。 |
| RDP 與 VNC | 在瀏覽器中開啟遠端桌面，使用工作階段控制、剪貼簿工具及鍵盤快捷鍵。目標必須提供可連線的 RDP 或 VNC 服務。 |
| 資料庫用戶端 | 連線至 PostgreSQL、MySQL/MariaDB、SQL Server、Redis 和 MongoDB，依引擎使用資料瀏覽器，以及可用的查詢、編輯與備份工具。 |
| Docker | 加入既有的 SSH 主機、探索容器、查看資源用量，以及操作容器、Compose 專案、映像檔、磁碟區與網路。可使用應用程式範本，或支援的自訂映像檔與 Compose 部署流程。 |
| 網路路徑 | 選擇可用的區域代理路線、設定自己的代理伺服器，或使用 SSH 跳板主機。 |
| 共享工作區 | 在個人與團隊工作區之間切換、邀請成員，並授予特定資源的存取權限。 |
| AI 與 MCP | 在終端機或資料庫工作旁尋求 AI 協助，或讓 MCP 用戶端連線至你授權的資源。 |
| 加密維運手冊與雲端儲存 | 整理工作文件、以獨立密碼加密敏感的維運手冊，並在可用的儲存空間中管理檔案。 |

可用協定、Docker 操作、資料庫寫入、AI 用量與儲存空間，取決於你的帳戶、工作區權限和連線目標的服務。介面會顯示目前工作階段可使用的功能。

## 由你掌握的加密保護與存取控制

Bastrio 將加密儲存與清楚可見的帳戶、連線控制整合在一起：

- **連線認證資訊加密儲存。** 已儲存的連線密碼與私鑰使用 AES-256-GCM 靜態加密保護。
- **傳輸保護。** 透過 HTTPS 使用 Bastr.io。SSH/SFTP 與 FTPS 提供加密的遠端傳輸，請依目標選擇合適的安全協定。
- **帳戶保護。** 啟用雙因素驗證，並離線保管復原金鑰。重設密碼後，可透過復原流程重新取得加密連線認證資訊的存取權。
- **加密維運手冊。** 為敏感筆記選擇加密模式並設定獨立的文件密碼。在編輯器中確認加密與儲存，並妥善保管文件密碼。
- **可控的 AI 存取。** MCP API 金鑰可選擇權限、設定到期時間，並撤銷存取。在允許敏感操作前，請檢查瀏覽器中的授權請求，並透過工作區介面管理伺服器認證資訊。

這些保護會與遠端系統本身的權限和安全設定共同發揮作用。請勿將復原資料與實際使用的認證資訊放入共享文件、螢幕截圖或 AI 對話。

## WebSSH、資料庫與 Docker 工具的替代方案

如果你的主要需求是在瀏覽器中以共享工作流程操作多種遠端資源，Bastrio 值得納入評估。無論你正在尋找 Termius 替代方案、FinalShell 或 Xshell 的瀏覽器替代工具、Navicat 類型的資料庫用戶端，或是透過 SSH 管理 Docker 的 Portainer 替代方案，都可以從實際要完成的任務出發。

| 常見比較工具 | 適合考慮 Bastrio 的情境 | 詳細指南 |
| --- | --- | --- |
| Termius、FinalShell、MobaXterm、Xshell、SecureCRT 與 PuTTY | 希望在瀏覽器中使用 SSH、儲存主機、分割工作階段，並就近操作檔案。若依賴桌面指令碼或 X11，請另外確認相關需求。 | [SSH 工具與瀏覽器工作區](../articles/zh-TW/ssh-tools-browser-workspace.md) |
| WinSCP、FileZilla、Xftp 與 Cyberduck | 希望在遠端工作階段旁完成 SFTP 或 FTP/FTPS 傳輸與文字編輯。 | [FTP/SFTP 工具與工作流程](../articles/zh-TW/ftp-sftp-tools-browser-workflow.md) |
| Navicat、DBeaver、DataGrip、pgAdmin、Redis Insight 與 MongoDB Compass | 希望在主機工作區旁使用瀏覽器資料庫用戶端。請依引擎、查詢、編輯和備份需求選擇。 | [遠端資料庫工具比較](../articles/zh-TW/remote-database-tools-comparison.md) |
| Apache Guacamole、TeamViewer、AnyDesk 與 ToDesk | 需要透過瀏覽器存取既有的 RDP/VNC 目標。有人值守的遠端協助與桌面閘道有不同的連線條件。 | [瀏覽器遠端桌面工具](../articles/zh-TW/browser-remote-desktop-tools.md) |
| Portainer、Dockge 與 Docker Desktop | 希望透過既有的 SSH 主機管理遠端 Docker 和 Compose 資源。本機容器開發與叢集管理則需要另外評估。 | [依情境比較 Docker 管理工具](../articles/zh-TW/docker-management-tools-by-scenario.md) |
| MCP 與 SSH、資料庫、Docker 工具的整合流程 | 希望 AI 用戶端在權限與操作核准機制下，探索並操作已授權的資源。 | [MCP 遠端管理](../articles/zh-TW/mcp-remote-management-tools.md) |

以上比較著重工作方式。功能涵蓋範圍會因產品、版本與設定而異；各篇指南也說明了哪些情境可能更適合使用專門工具。

## 在瀏覽器中開始使用

1. 前往 [bastr.io](https://bastr.io/zh-TW/)。訪客連線開放時可用於臨時工作階段；登入後則可儲存並整理工作資源。
2. 在**快速連線（Quick Connect）**中選擇連線類型並輸入目標，或在**主機（Hosts）**中新增連線。密碼與私鑰只應填入連線表單。
3. 如果目標需要特定的網路路徑，請選擇代理伺服器或 SSH 跳板主機。
4. 開啟工作階段，透過**檔案（Files）**、資料庫面板或 **Docker** 接續下一項任務，並使用版面配置控制安排相關工作階段。
5. 團隊協作時，請選擇正確的工作區並共享成員需要的資源。在將帳戶用於日常存取之前，請啟用雙因素驗證並保存復原資料。

訪客存取有個別的開放條件與使用額度。儲存主機、團隊功能及部分工具需要登入或符合條件的帳戶。

## 透過 SSH 管理 Docker

在工作區開啟 **Docker**，並選擇你有權限存取的 SSH 主機。Docker 檢視將容器、Compose、映像檔、磁碟區、網路與任務進度集中呈現。你可以檢查容器狀態與資源用量、執行支援的生命週期操作，並從可用的應用程式範本、自訂映像檔或支援的 Compose 設定開始部署。

若目標尚未安裝 Docker，介面可在支援的 Linux 主機上引導安裝；請先檢視並確認建議的操作。實際可用性取決於主機、你的權限及目前開放的功能。你可以參考 [Docker 比較指南](../articles/zh-TW/docker-management-tools-by-scenario.md)中的實際評估流程。

## 透過 MCP 連線 AI 用戶端

Bastrio 支援 Claude Code、Codex、Cursor、VS Code 等用戶端透過 Model Context Protocol（MCP，模型上下文協定）連線。MCP 可搭配內建 AI 助手，讓你選擇的用戶端使用已授權的主機、檔案、資料庫與網路路徑。

1. 在工作區開啟**工具 → MCP API 金鑰（Tools → MCP API Keys）**。
2. 依用戶端需求設定權限與到期時間，並建立金鑰。
3. 選擇用戶端，依照該頁面顯示的說明設定連線。
4. 將金鑰存放在用戶端支援的機密資訊或環境變數設定中。在瀏覽器中檢查授權請求，並在不再需要時撤銷存取。

請使用帳戶中顯示的連線端點。可用工具取決於授予的權限，應由用戶端向 MCP 服務探索取得。閱讀 [MCP 指南](../articles/zh-TW/mcp-remote-management-tools.md)，了解它如何配合 SSH、資料庫與 Docker 工作。

## 六篇實用指南，十種語言

[指南文庫](../articles/README.md)收錄六篇已發布工具比較文章，提供英文、簡體中文、繁體中文、西班牙文、德文、法文、日文、韓文、馬來文與俄文版本。各版本保留既有文章的正文、插圖、常見問題，以及對應的 Bastr.io 原文連結。

[English guides](../articles/en/README.md) · [简体中文指南](../articles/zh/README.md) · [繁體中文指南](../articles/zh-TW/README.md) · [日本語](../articles/ja/README.md) · [한국어](../articles/ko/README.md) · [Español](../articles/es/README.md) · [Deutsch](../articles/de/README.md) · [Français](../articles/fr/README.md) · [Bahasa Melayu](../articles/ms/README.md) · [Русский](../articles/ru/README.md)

## 常見問題

### Bastrio 是什麼？

Bastrio 是整合 WebSSH、檔案傳輸、RDP/VNC、資料庫、Docker 管理、共享資源與 AI 輔助的瀏覽器工作區，適合需要跨多個遠端系統工作的開發者與維運人員。

### Bastrio 可以取代 Termius、FinalShell 或 MobaXterm 嗎？

Bastrio 提供在瀏覽器中處理常見 SSH 與檔案管理任務的工作方式。更換工具前，請評估你依賴的桌面功能，例如本機 Shell 整合、巨集或 X11。[SSH 工具比較](../articles/zh-TW/ssh-tools-browser-workspace.md)可協助你依情境選擇。

### Bastrio 可以作為 Navicat 或 DBeaver 的瀏覽器替代方案嗎？

Bastrio 可處理 PostgreSQL、MySQL/MariaDB、SQL Server、Redis 和 MongoDB 的常見遠端資料庫工作。可用操作依引擎與權限而異。進階建模、同步與專門的開發流程，仍應依你的實際需求評估。

### Bastrio 是 Portainer 的替代方案嗎？

如果你希望在 SSH、檔案與資料庫旁管理 Docker 主機和 Compose，Bastrio 提供透過既有 SSH 連線操作的瀏覽器工作流程。請結合你的環境與部署需求，參考 [Docker 指南](../articles/zh-TW/docker-management-tools-by-scenario.md)進行比較。

### 需要安裝桌面用戶端嗎？

你可以從支援的瀏覽器使用工作區。目標仍須提供可連線的 SSH、檔案傳輸、遠端桌面或資料庫服務，並具備有效的存取認證資訊。

### 連線認證資訊與敏感筆記如何受到保護？

已儲存的連線認證資訊使用 AES-256-GCM 靜態加密，瀏覽器則透過 HTTPS 存取 Bastr.io。敏感維運手冊支援使用獨立文件密碼加密儲存；雙因素驗證、復原資料與資源權限則提供額外的存取控制。

### 可以不註冊帳戶就開始使用嗎？

首頁提供訪客連線時即可使用。訪客存取、支援協定與可用時長可能調整；登入後可儲存連線，並使用帳戶開放的工具。

## 聯絡方式與專案資訊

官方網站：[bastr.io](https://bastr.io/zh-TW/) · 支援信箱：[sup@bastr.io](mailto:sup@bastr.io) · [回報問題](https://github.com/cihalqe/bastrio/issues)

本儲存庫收錄 Bastrio 的公開產品文件與使用指南，歡迎提出建議與修正。請在 Issue 和 Pull Request 中只分享不含敏感資訊的範例。

授權條款：[GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html)。
