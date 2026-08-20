<p align="center"><a href="https://bastr.io/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a></p>

<p align="center">안전한 원격 액세스, 인프라 작업 및 협업을 위한 브라우저 워크스페이스.</p>

<p align="center"><a href="https://bastr.io/"><strong>bastr.io</strong></a> &nbsp;|&nbsp; <a href="https://www.gnu.org/licenses/gpl-3.0.html"><img src="https://img.shields.io/badge/license-GPL--3.0--only-2b82f0.svg" alt="GPL-3.0-only" /></a></p>

<p align="center"><a href="../../README.md">English</a> | <a href="README.zh-CN.md">简体中文</a> | <a href="README.zh-TW.md">繁體中文</a> | <a href="README.ja.md">日本語</a> | <strong>한국어</strong> | <a href="README.es.md">Español</a> | <a href="README.de.md">Deutsch</a> | <a href="README.fr.md">Français</a> | <a href="README.pt.md">Português</a> | <a href="README.ar.md">العربية</a></p>

## 원격 인프라를 위한 하나의 브라우저 워크스페이스

[Bastrio](https://bastr.io/)는 **온라인 SSH**, SFTP, FTP/FTPS, RDP, VNC 및 데이터베이스 연결을 하나의 브라우저 워크스페이스로 모읍니다. 웹 SSH 터미널, 온라인 파일 관리자, 브라우저 데이터베이스 클라이언트, 팀용 원격 서버 관리 공간으로 사용할 수 있습니다.

![Bastrio 온라인 SSH 및 브라우저 원격 액세스](../images/readme/ssh-online-guest.png)

## 주요 기능

- **브라우저에서 연결:** 온라인 SSH 터미널, SFTP/FTP/FTPS 파일 작업, RDP 및 VNC 원격 데스크톱.
- **통합 데이터베이스 도구:** PostgreSQL, MySQL/MariaDB, SQL Server, Redis, MongoDB를 같은 워크스페이스에서 연결합니다.
- **연결 구성:** 저장된 연결, 폴더, 유형 필터, 최근 연결, 다중 세션 및 분할 레이아웃.
- **네트워크 경로 선택:** 지역별 프록시 IP, 사용자 지정 프록시 또는 SSH 점프 호스트로 비공개 인프라에 접근합니다.
- **AI 지원:** 터미널과 데이터베이스 옆에서 AI 어시스턴트가 출력 해석, 명령 작성 및 일상 작업을 돕습니다.
- **협업 워크스페이스:** 워크스페이스와 공유 리소스로 팀의 연결 맥락을 유지합니다.
- **암호화된 작업 문서:** 민감한 메모, 초안 및 작업 텍스트를 워크스페이스에서 암호화하여 저장합니다.

<p align="center"><img src="../images/readme/ssh-online-terminal.png" width="49%" alt="Bastrio 온라인 SSH 터미널" /> <img src="../images/readme/connection-types.png" width="49%" alt="Bastrio 연결 유형" /></p>

<p align="center"><img src="../images/readme/remote-workspace.png" width="49%" alt="Bastrio 원격 워크스페이스" /> <img src="../images/readme/sftp-file-browser.png" width="49%" alt="Bastrio SFTP 파일 브라우저" /></p>

<p align="center"><img src="../images/readme/proxy-region-picker.png" width="49%" alt="Bastrio 프록시 지역 선택" /> <img src="../images/readme/split-workspace.png" width="49%" alt="Bastrio 분할 워크스페이스" /></p>

<p align="center"><img src="../images/readme/postgresql-workspace.png" width="49%" alt="Bastrio PostgreSQL 워크스페이스" /> <img src="../images/readme/encrypted-operations-documents.png" width="49%" alt="Bastrio 암호화 작업 문서" /></p>

<p align="center"><img src="../images/readme/recovery-key.png" width="49%" alt="Bastrio 복구 키" /></p>

## 제어 가능한 네트워크 경로

Bastrio에서는 작업에 맞는 경로로 브라우저 원격 액세스를 사용할 수 있습니다. 출구 지역이 필요하면 **프록시 IP**를 선택하고, 경로를 직접 제어하려면 사용자 지정 프록시를 사용하며, 직접 공개되지 않은 인프라에는 **SSH 점프 호스트**를 사용합니다. 모든 선택은 연결 설정 안에 있습니다.

## 집중과 협업을 위한 원격 작업

Bastrio는 서버, 파일, 데스크톱 및 데이터베이스를 자주 오가는 개발자, 운영 담당자 및 팀을 위한 원격 워크스페이스입니다. 워크스페이스와 공유 리소스가 맥락을 보존하고, 다중 세션과 분할 레이아웃이 관련 작업을 함께 보여 주며, AI 어시스턴트는 터미널 또는 데이터베이스 작업 가까이에 있습니다.

## 프라이버시 설계

자격 증명과 비공개 워크스페이스 콘텐츠는 전송 중과 저장 시 암호화됩니다. Bastrio는 권한이 부여된 작업에 필요한 경우에만 서버의 휘발성 메모리에서 자격 증명을 일시적으로 복호화합니다. 평문은 디스크나 로그에 기록되지 않습니다. 사용자에게 보이는 모든 액세스에는 활성 인증 세션이 필요합니다. 세션이 만료되거나 취소되면 암호화된 볼트에 더 이상 접근하거나 복호화할 수 없습니다. 복구 키는 한 번만 표시되며 비밀번호 재설정 후 암호화된 자격 증명을 복원하는 데 필요합니다. 키가 없으면 암호화된 볼트를 복원하거나 읽을 수 있는 형식으로 내보낼 수 없습니다.

## Marketplace, 예정됨

Bastrio는 관리형 서버 및 프록시 IP 서비스를 위한 Marketplace를 준비하고 있습니다. 이는 향후 릴리스 계획이며 현재 제공되는 서비스가 아닙니다.

## 시작하기

1. [bastr.io](https://bastr.io/)에서 Bastrio 원격 워크스페이스를 엽니다.
2. SSH, 파일 전송, 원격 데스크톱 또는 데이터베이스 연결을 선택합니다.
3. 필요할 때 네트워크 경로를 고르고 연결을 저장해 구성합니다.

## 자주 묻는 질문

### Bastrio는 웹 SSH 터미널인가요?

예. Bastrio는 브라우저에서 온라인 SSH를 제공하며 파일 전송, 원격 데스크톱, 데이터베이스, 프록시 및 워크스페이스 도구를 함께 제공합니다.

### 프록시 IP, 사용자 지정 프록시 및 SSH 점프 호스트를 사용할 수 있나요?

예. 지역별 프록시 IP 선택, 사용자 지정 프록시 구성 및 SSH 점프 호스트를 지원합니다.

### 팀이 같은 환경에서 협업할 수 있나요?

예. 워크스페이스와 공유 리소스는 원격 인프라 작업을 구성하고 협업하기 쉽게 만듭니다.

## 문의

이메일: [sup@bastr.io](mailto:sup@bastr.io)

## 기여

기여와 이슈 보고를 환영합니다. 제안은 사용자에게 보이는 동작에 집중하고, 이슈나 pull request에 자격 증명 또는 비공개 연결 데이터를 포함하지 마십시오.

## 라이선스

Bastrio는 [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html)으로 배포됩니다.
