<p align="center"><a href="https://bastr.io/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a></p>

<p align="center">安全なリモートアクセス、インフラ作業、コラボレーションのためのブラウザワークスペース。</p>

<p align="center"><a href="https://bastr.io/"><strong>bastr.io</strong></a> &nbsp;|&nbsp; <a href="https://www.gnu.org/licenses/gpl-3.0.html"><img src="https://img.shields.io/badge/license-GPL--3.0--only-2b82f0.svg" alt="GPL-3.0-only" /></a></p>

<p align="center"><a href="../../README.md">English</a> | <a href="README.zh-CN.md">简体中文</a> | <a href="README.zh-TW.md">繁體中文</a> | <strong>日本語</strong> | <a href="README.ko.md">한국어</a> | <a href="README.es.md">Español</a> | <a href="README.de.md">Deutsch</a> | <a href="README.fr.md">Français</a> | <a href="README.pt.md">Português</a> | <a href="README.ar.md">العربية</a></p>

## リモートインフラのためのブラウザワークスペース

[Bastrio](https://bastr.io/) は、**オンライン SSH**、SFTP、FTP/FTPS、RDP、VNC、データベース接続を一つのブラウザワークスペースにまとめます。Web SSH ターミナル、オンラインファイルマネージャー、ブラウザデータベースクライアント、そしてチームのリモートサーバー管理スペースとして使えます。

![Bastrio のオンライン SSH とブラウザリモートアクセス](../images/readme/ssh-online-guest.png)

## 主な機能

- **ブラウザから接続：** オンライン SSH ターミナル、SFTP/FTP/FTPS のファイル操作、RDP と VNC のリモートデスクトップ。
- **統合データベースツール：** PostgreSQL、MySQL/MariaDB、SQL Server、Redis、MongoDB を同じワークスペースで接続。
- **接続を整理：** 保存済み接続、フォルダー、種類フィルター、最近の接続、複数セッション、分割レイアウト。
- **ネットワーク経路を選択：** 地域別のプロキシ IP、カスタムプロキシ、または SSH ジャンプホストで非公開インフラへアクセス。
- **AI アシスタント：** ターミナルやデータベースの横で出力の説明、コマンド作成、日常作業を支援。
- **共同ワークスペース：** ワークスペースと共有リソースでチームの接続コンテキストを保ちます。
- **暗号化された作業文書：** 機密メモ、下書き、作業テキストをワークスペース内で暗号化して保存。

<p align="center"><img src="../images/readme/ssh-online-terminal.png" width="49%" alt="Bastrio のオンライン SSH ターミナル" /> <img src="../images/readme/connection-types.png" width="49%" alt="Bastrio の接続タイプ" /></p>

<p align="center"><img src="../images/readme/remote-workspace.png" width="49%" alt="Bastrio のリモートワークスペース" /> <img src="../images/readme/sftp-file-browser.png" width="49%" alt="Bastrio の SFTP ファイルブラウザー" /></p>

<p align="center"><img src="../images/readme/proxy-region-picker.png" width="49%" alt="Bastrio のプロキシ地域選択" /> <img src="../images/readme/split-workspace.png" width="49%" alt="Bastrio の分割ワークスペース" /></p>

<p align="center"><img src="../images/readme/postgresql-workspace.png" width="49%" alt="Bastrio の PostgreSQL ワークスペース" /> <img src="../images/readme/encrypted-operations-documents.png" width="49%" alt="Bastrio の暗号化作業文書" /></p>

<p align="center"><img src="../images/readme/recovery-key.png" width="49%" alt="Bastrio のリカバリーキー" /></p>

## 制御できるネットワーク経路

Bastrio では、作業に合う経路でブラウザリモートアクセスを利用できます。出口地域が必要なら**プロキシ IP**、経路を制御したいならカスタムプロキシ、直接公開されていない環境には **SSH ジャンプホスト**を選びます。これらは接続設定にまとまっており、別のツールは不要です。

## 集中できる共同リモート作業

Bastrio は、サーバー、ファイル、デスクトップ、データベースを行き来する開発者、運用担当者、チーム向けのリモートワークスペースです。ワークスペースと共有リソースが文脈を保ち、複数セッションと分割レイアウトが関連作業を表示し続け、AI アシスタントは作業のそばにいます。

## プライバシー設計

認証情報と非公開ワークスペースの内容は、転送中と保存時に暗号化されます。Bastrio は許可された操作に必要な場合のみ、サーバーの揮発性メモリで認証情報を一時的に復号します。平文がディスクやログに書き込まれることはありません。ユーザーに表示されるすべてのアクセスには、有効な認証済みセッションが必要です。セッションの期限切れまたは失効後は、暗号化ボルトへのアクセスや復号は一切できません。リカバリーキーは一度だけ表示され、パスワードリセット後に暗号化された認証情報を復元するために必要です。このキーがなければ、暗号化ボルトは復元も可読形式でのエクスポートもできません。

## Marketplace（予定）

Bastrio はマネージドサーバーとプロキシ IP サービスの Marketplace を準備しています。これらは将来のリリースに向けた計画であり、現在利用できるサービスではありません。

## はじめる

1. [bastr.io](https://bastr.io/) で Bastrio リモートワークスペースを開きます。
2. SSH、ファイル転送、リモートデスクトップ、またはデータベース接続を選びます。
3. 必要に応じてネットワーク経路を選び、接続を保存・整理します。

## よくある質問

### Bastrio は Web SSH ターミナルですか？

はい。Bastrio はブラウザでオンライン SSH を提供し、ファイル転送、リモートデスクトップ、データベース、プロキシ、ワークスペースの機能を統合します。

### プロキシ IP、カスタムプロキシ、SSH ジャンプホストは使えますか？

はい。地域別プロキシ IP、カスタムプロキシ設定、SSH ジャンプホストをサポートしています。

### チームで同じ環境を共有できますか？

はい。ワークスペースと共有リソースは、リモートインフラ作業を整理し、共同作業しやすくするためのものです。

## 連絡先

メール: [sup@bastr.io](mailto:sup@bastr.io)

## コントリビューション

貢献と issue 報告を歓迎します。提案はユーザーに見える動作に集中させ、認証情報や非公開の接続データを issue や pull request に含めないでください。

## ライセンス

Bastrio は [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html) で公開されています。
