<p align="center">
  <a href="https://bastr.io/ko/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a>
</p>

# Bastrio — 브라우저에서 사용하는 WebSSH, 원격 데스크톱, 데이터베이스, Docker

[Bastrio(Bastr.io)](https://bastr.io/ko/)는 원격 서버 관리를 위한 브라우저 워크스페이스입니다. 온라인 SSH 터미널을 열고, SFTP로 파일을 전송하고, RDP나 VNC 데스크톱에 연결하고, 데이터베이스와 Docker 호스트를 한곳에서 관리할 수 있습니다. 저장된 연결, 분할 화면, 공유 워크스페이스, AI 지원으로 관련 작업을 이어서 처리하면서 자격 증명 암호화 저장과 계정 보호 기능도 함께 사용할 수 있습니다.

[워크스페이스 열기](https://bastr.io/workspace/) · [가이드 읽기](../articles/README.md) · [웹사이트](https://bastr.io/ko/)

[English](../../README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [日本語](README.ja.md) · 한국어 · [Español](README.es.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · [Português](README.pt.md) · [العربية](README.ar.md)

## 작업 흐름을 이어 주는 워크스페이스

호스트에 연결해 터미널을 열고, 설정 파일을 살펴보고, 데이터베이스와 컨테이너 상태를 확인하는 작업을 여러 앱에서 연결 환경을 다시 구성할 필요 없이 이어서 처리할 수 있습니다. Bastrio는 호스트 사이드바, 세션 탭, 분할 레이아웃, 파일 및 데이터베이스 패널, Docker 및 AI 전용 화면을 작업 가까이에 배치합니다.

![SSH 터미널과 SFTP 파일 관리자를 분할 화면으로 보여 주는 Bastrio 브라우저 워크스페이스](../images/readme/split-workspace.png)

| 기능 영역 | 화면에서 할 수 있는 작업 |
| --- | --- |
| 호스트와 세션 | 연결 저장, 폴더 정리, 연결 유형별 필터링, 최근 세션 다시 열기, 탭 및 분할 화면 배치. |
| WebSSH와 원격 명령 | SSH 비밀번호 또는 개인 키 인증, 브라우저 터미널, 빠른 명령, 검색 및 다시 연결 기능. 활성화된 환경에서는 WinRM과 Telnet 연결 유형도 사용할 수 있습니다. |
| SFTP, FTP, FTPS | 디렉터리 탐색, 파일 업로드와 다운로드, 폴더 만들기, 파일 이름 변경, 터미널 옆에서 지원되는 텍스트 파일 편집. |
| RDP와 VNC | 브라우저에서 원격 데스크톱에 연결하고 세션 제어, 클립보드 도구, 키보드 단축키 사용. 대상에는 접근 가능한 RDP 또는 VNC 서비스가 필요합니다. |
| 데이터베이스 클라이언트 | PostgreSQL, MySQL/MariaDB, SQL Server, Redis, MongoDB에 연결. 해당 엔진의 데이터 탐색 기능과 제공되는 쿼리, 편집, 백업 도구를 사용할 수 있습니다. |
| Docker | 기존 SSH 호스트 추가, 컨테이너 검색, 리소스 사용량 확인, 컨테이너·Compose 프로젝트·이미지·볼륨·네트워크 관리. 애플리케이션 템플릿이나 지원되는 사용자 지정 이미지 및 Compose 배포 흐름을 사용할 수 있습니다. |
| 네트워크 경로 | 사용 가능한 지역별 프록시 경로 선택, 자체 프록시 설정, SSH 점프 호스트 사용. |
| 공유 워크스페이스 | 개인 및 팀 워크스페이스 전환, 구성원 초대, 선택한 리소스에 대한 접근 권한 부여. |
| AI와 MCP | 터미널이나 데이터베이스 작업 중 AI의 도움을 받거나, 허용한 리소스에 MCP 클라이언트로 연결할 수 있습니다. |
| 암호화 런북과 클라우드 스토리지 | 작업 문서를 정리하고, 민감한 런북(운영 절차서)을 별도 비밀번호로 암호화하며, 사용 가능한 저장 공간에서 파일을 관리합니다. |

사용 가능한 프로토콜, Docker 작업, 데이터베이스 쓰기, AI 사용량 및 저장 공간은 계정, 워크스페이스 권한, 연결 대상 서비스에 따라 달라집니다. 현재 세션에서 사용할 수 있는 기능은 화면에 표시됩니다.

## 직접 관리하는 암호화와 접근 제어

Bastrio는 암호화 저장과 함께 계정 및 연결 보호 설정을 화면에서 확인하고 관리할 수 있게 합니다.

- **연결 자격 증명 암호화.** 저장된 연결 비밀번호와 개인 키는 AES-256-GCM으로 저장 시 암호화됩니다.
- **전송 보호.** Bastr.io에는 HTTPS로 접속하세요. SSH/SFTP와 FTPS는 원격 통신을 암호화하므로 대상에 적합한 안전한 프로토콜을 선택하세요.
- **계정 보호.** 2단계 인증을 활성화하고 복구 키를 오프라인에 보관하세요. 비밀번호를 재설정한 후에는 복구 절차를 통해 암호화된 연결 자격 증명에 다시 접근할 수 있습니다.
- **런북 암호화.** 민감한 메모는 암호화 모드를 선택하고 별도의 문서 비밀번호를 설정하세요. 편집기에서 암호화 및 저장 여부를 확인하고 문서 비밀번호를 안전하게 보관하세요.
- **AI 접근 제어.** MCP API 키의 권한과 만료일을 설정하고 접근을 취소할 수 있습니다. 민감한 작업을 허용하기 전에 브라우저의 승인 요청을 검토하고, 서버 자격 증명은 워크스페이스 화면에서 관리하세요.

이러한 보호 기능은 원격 시스템의 권한 및 보안 설정과 함께 작동합니다. 복구 정보나 실제 자격 증명을 공유 문서, 스크린샷, AI 대화에 포함하지 마세요.

## WebSSH, 데이터베이스, Docker 도구의 대안

여러 종류의 원격 리소스를 브라우저의 공유 작업 흐름으로 관리하고 싶다면 Bastrio를 검토할 수 있습니다. Termius 대안, FinalShell이나 Xshell을 대신할 브라우저 도구, Navicat과 같은 데이터베이스 클라이언트, SSH로 Docker를 관리하는 Portainer 대안을 비교하고 있다면 실제로 완료해야 하는 작업을 기준으로 선택하세요.

| 비교할 수 있는 도구 | Bastrio를 고려할 만한 상황 | 자세한 가이드 |
| --- | --- | --- |
| Termius, FinalShell, MobaXterm, Xshell, SecureCRT, PuTTY | 브라우저 SSH, 호스트 저장, 세션 분할, 인접한 파일 도구가 필요한 경우. 데스크톱 스크립트 기능이나 X11 요구 사항은 별도로 확인하세요. | [SSH 도구와 브라우저 워크스페이스](../articles/ko/ssh-tools-browser-workspace.md) |
| WinSCP, FileZilla, Xftp, Cyberduck | 원격 세션 옆에서 SFTP 또는 FTP/FTPS 전송과 텍스트 편집을 수행하려는 경우. | [FTP/SFTP 도구와 작업 흐름](../articles/ko/ftp-sftp-tools-browser-workflow.md) |
| Navicat, DBeaver, DataGrip, pgAdmin, Redis Insight, MongoDB Compass | 호스트 작업 화면에서 브라우저 데이터베이스 클라이언트를 함께 사용하려는 경우. 엔진, 쿼리, 편집, 백업 요구 사항을 기준으로 선택하세요. | [원격 데이터베이스 도구 비교](../articles/ko/remote-database-tools-comparison.md) |
| Apache Guacamole, TeamViewer, AnyDesk, ToDesk | 기존 RDP/VNC 대상에 브라우저로 접근해야 하는 경우. 상대방이 참여하는 원격 지원과 데스크톱 게이트웨이는 연결 조건이 다릅니다. | [브라우저 원격 데스크톱 도구](../articles/ko/browser-remote-desktop-tools.md) |
| Portainer, Dockge, Docker Desktop | 기존 SSH 호스트를 통해 원격 Docker 및 Compose 리소스를 관리하려는 경우. 로컬 컨테이너 개발과 클러스터 관리는 별도의 선택 기준으로 검토하세요. | [사용 시나리오별 Docker 관리 도구](../articles/ko/docker-management-tools-by-scenario.md) |
| SSH·데이터베이스·Docker 도구와 함께 사용하는 MCP 작업 흐름 | 권한과 승인 절차에 따라 AI 클라이언트가 허용된 리소스를 검색하고 작업하도록 하려는 경우. | [MCP 원격 관리](../articles/ko/mcp-remote-management-tools.md) |

위 비교는 작업 방식을 기준으로 합니다. 기능 범위는 제품, 에디션, 설정에 따라 달라지며, 각 가이드에서는 전문 도구가 더 적합한 상황도 설명합니다.

## 브라우저에서 시작하기

1. [bastr.io](https://bastr.io/ko/)에 접속합니다. 게스트 연결이 제공되면 임시 세션에 이용할 수 있으며, 로그인하면 연결과 작업 리소스를 저장하고 정리할 수 있습니다.
2. **빠른 연결(Quick Connect)**에서 연결 유형을 선택하고 대상을 입력하거나 **호스트(Hosts)**에 추가합니다. 비밀번호와 개인 키는 연결 양식에만 입력하세요.
3. 대상에 특정 네트워크 경로가 필요하면 프록시 또는 SSH 점프 호스트를 선택합니다.
4. 세션을 엽니다. **파일(Files)**, 데이터베이스 패널 또는 **Docker**에서 다음 작업을 이어서 진행하고, 레이아웃 기능으로 관련 세션을 배치합니다.
5. 팀 작업에서는 알맞은 워크스페이스를 선택하고 구성원에게 필요한 리소스를 공유합니다. 계정을 일상적인 접근 수단으로 사용하기 전에 2단계 인증을 활성화하고 복구 정보를 보관하세요.

게스트 접근에는 별도의 제공 조건과 사용 한도가 있습니다. 호스트 저장, 팀 기능 및 일부 도구를 사용하려면 로그인하거나 해당 기능을 이용할 수 있는 계정이 필요합니다.

## SSH를 통한 Docker 관리

워크스페이스에서 **Docker**를 열고 접근 권한이 있는 SSH 호스트를 선택합니다. Docker 화면에는 컨테이너, Compose, 이미지, 볼륨, 네트워크, 작업 진행 상황이 한곳에 표시됩니다. 컨테이너 상태와 리소스 사용량을 확인하고 지원되는 수명 주기 작업을 실행할 수 있으며, 제공되는 애플리케이션 템플릿, 사용자 지정 이미지 또는 지원되는 Compose 설정으로 배포를 시작할 수 있습니다.

Docker가 설치되어 있지 않다면 지원되는 Linux 호스트에서 화면의 안내에 따라 설치할 수 있습니다. 먼저 제안된 작업을 검토하고 확인해야 합니다. 사용 가능 여부는 호스트, 권한, 현재 제공되는 기능에 따라 달라집니다. 실제 평가 절차는 [Docker 비교 가이드](../articles/ko/docker-management-tools-by-scenario.md)를 참고하세요.

## MCP로 AI 클라이언트 연결하기

Bastrio는 Claude Code, Codex, Cursor, VS Code 등의 클라이언트에서 Model Context Protocol(MCP)로 연결하는 방식을 지원합니다. MCP는 내장 AI 어시스턴트를 보완하며, 선택한 클라이언트가 허용된 호스트, 파일, 데이터베이스, 네트워크 경로를 다룰 수 있게 합니다.

1. 워크스페이스에서 **도구 → MCP API 키(Tools → MCP API Keys)**를 엽니다.
2. 클라이언트에 필요한 권한과 만료일을 설정해 키를 생성합니다.
3. 클라이언트를 선택하고 해당 페이지의 연결 안내를 따릅니다.
4. 키는 클라이언트에서 지원하는 시크릿 또는 환경 변수 설정에 보관하세요. 브라우저에서 승인 요청을 검토하고 더 이상 필요하지 않은 접근 권한은 취소하세요.

계정 화면에 표시된 엔드포인트를 사용하세요. 사용할 수 있는 도구는 부여된 권한에 따라 달라지므로 클라이언트가 MCP 서비스에서 도구를 검색해야 합니다. SSH, 데이터베이스, Docker 작업과 함께 활용하는 예는 [MCP 가이드](../articles/ko/mcp-remote-management-tools.md)에서 확인할 수 있습니다.

## 실용 가이드 6편, 10개 언어

[가이드 라이브러리](../articles/README.md)에는 이미 공개된 도구 비교 글 6편의 영어, 중국어 간체, 중국어 번체, 스페인어, 독일어, 프랑스어, 일본어, 한국어, 말레이어, 러시아어 버전이 있습니다. 각 버전은 기존 글의 본문, 그림, FAQ와 Bastr.io 원문 링크를 유지합니다.

[English guides](../articles/en/README.md) · [简体中文指南](../articles/zh/README.md) · [繁體中文指南](../articles/zh-TW/README.md) · [日本語](../articles/ja/README.md) · [한국어](../articles/ko/README.md) · [Español](../articles/es/README.md) · [Deutsch](../articles/de/README.md) · [Français](../articles/fr/README.md) · [Bahasa Melayu](../articles/ms/README.md) · [Русский](../articles/ru/README.md)

## 자주 묻는 질문

### Bastrio는 무엇인가요?

Bastrio는 WebSSH, 파일 전송, RDP/VNC, 데이터베이스, Docker 관리, 공유 리소스, AI 지원을 통합한 브라우저 워크스페이스입니다. 여러 원격 시스템을 함께 다루는 개발자와 운영 담당자를 위해 설계되었습니다.

### Bastrio가 Termius, FinalShell, MobaXterm을 대체할 수 있나요?

Bastrio는 일반적인 SSH 및 파일 관리 작업을 브라우저에서 처리하는 흐름을 제공합니다. 도구를 바꾸기 전에 로컬 셸 통합, 매크로, X11 등 자주 사용하는 데스크톱 기능의 요구 사항을 확인하세요. [SSH 도구 비교](../articles/ko/ssh-tools-browser-workspace.md)에서 상황에 맞게 선택하는 방법을 살펴볼 수 있습니다.

### Bastrio를 Navicat이나 DBeaver의 브라우저 대안으로 사용할 수 있나요?

PostgreSQL, MySQL/MariaDB, SQL Server, Redis, MongoDB의 일반적인 원격 데이터베이스 작업에 사용할 수 있습니다. 가능한 작업은 엔진과 권한에 따라 달라집니다. 고급 모델링, 동기화, 전문적인 개발 흐름은 실제 요구 사항에 맞춰 평가하세요.

### Bastrio는 Portainer의 대안인가요?

SSH, 파일, 데이터베이스 작업과 함께 Docker 호스트 및 Compose를 관리하려는 사용자에게 Bastrio는 기존 SSH 연결을 활용하는 브라우저 작업 흐름을 제공합니다. [Docker 가이드](../articles/ko/docker-management-tools-by-scenario.md)를 참고해 환경과 배포 요구 사항에 맞는지 비교하세요.

### 데스크톱 클라이언트를 설치해야 하나요?

지원되는 브라우저에서 워크스페이스를 사용할 수 있습니다. 대상에는 접근 가능한 SSH, 파일 전송, 원격 데스크톱 또는 데이터베이스 서비스와 유효한 접근 자격 증명이 필요합니다.

### 연결 자격 증명과 민감한 메모는 어떻게 보호되나요?

저장된 연결 자격 증명은 AES-256-GCM으로 저장 시 암호화되며, 브라우저에서는 HTTPS로 Bastr.io에 접속합니다. 민감한 런북은 별도의 문서 비밀번호로 암호화해 저장할 수 있습니다. 2단계 인증, 복구 정보, 리소스 권한이 추가적인 제어 수단을 제공합니다.

### 계정 없이 시작할 수 있나요?

홈페이지에서 게스트 연결을 제공할 때 이용할 수 있습니다. 게스트 접근의 제공 여부, 프로토콜, 사용 시간 한도는 변경될 수 있습니다. 연결을 저장하고 계정에 제공되는 도구를 사용하려면 로그인하세요.

## 문의 및 프로젝트 정보

웹사이트: [bastr.io](https://bastr.io/ko/) · 지원: [sup@bastr.io](mailto:sup@bastr.io) · [문제 보고](https://github.com/cihalqe/bastrio/issues)

이 저장소에는 Bastrio의 공개 제품 문서와 가이드가 담겨 있습니다. 제안과 수정을 환영합니다. Issue와 Pull Request에는 민감한 정보가 없는 예시만 공유해 주세요.

라이선스: [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).
