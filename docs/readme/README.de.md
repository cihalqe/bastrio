<p align="center"><a href="https://bastr.io/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a></p>

<p align="center">Ein Browser-Arbeitsbereich für sicheren Fernzugriff, Infrastrukturarbeit und Zusammenarbeit.</p>

<p align="center"><a href="https://bastr.io/"><strong>bastr.io</strong></a> &nbsp;|&nbsp; <a href="https://www.gnu.org/licenses/gpl-3.0.html"><img src="https://img.shields.io/badge/license-GPL--3.0--only-2b82f0.svg" alt="GPL-3.0-only" /></a></p>

<p align="center"><a href="../../README.md">English</a> | <a href="README.zh-CN.md">简体中文</a> | <a href="README.zh-TW.md">繁體中文</a> | <a href="README.ja.md">日本語</a> | <a href="README.ko.md">한국어</a> | <a href="README.es.md">Español</a> | <strong>Deutsch</strong> | <a href="README.fr.md">Français</a> | <a href="README.pt.md">Português</a> | <a href="README.ar.md">العربية</a></p>

## Ein Arbeitsbereich für Remote-Infrastruktur

[Bastrio](https://bastr.io/) vereint **SSH online**, SFTP, FTP/FTPS, RDP, VNC und Datenbankverbindungen in einem Browser-Arbeitsbereich. Nutzen Sie es als Web-SSH-Terminal, Online-Dateimanager, Browser-Datenbankclient oder gemeinsamen Bereich für die Verwaltung entfernter Server.

![Bastrio SSH online und Browser-Fernzugriff](../images/readme/ssh-online-guest.png)

## Zentrale Funktionen

- **Im Browser verbinden:** Online-SSH-Terminal, Dateien über SFTP/FTP/FTPS sowie RDP- und VNC-Remote-Desktops.
- **Einheitliche Datenbankwerkzeuge:** PostgreSQL, MySQL/MariaDB, SQL Server, Redis und MongoDB im selben Arbeitsbereich.
- **Verbindungen organisieren:** gespeicherte Verbindungen, Ordner, Typfilter, zuletzt verwendete Verbindungen, mehrere Sitzungen und geteilte Ansichten.
- **Netzwerkweg wählen:** regionale Proxy-IP, eigener Proxy oder ein SSH-Jump-Host für nicht direkt erreichbare Infrastruktur.
- **KI-Unterstützung:** Der KI-Assistent hilft neben Terminal und Datenbank beim Erklären von Ausgaben, beim Erstellen von Befehlen und in der täglichen Arbeit.
- **Gemeinsam arbeiten:** Arbeitsbereiche und geteilte Ressourcen bewahren den Verbindungskontext für Teams.
- **Verschlüsselte Arbeitsdokumente:** Notizen, Entwürfe und sensible Arbeitstexte innerhalb des Arbeitsbereichs verschlüsseln und speichern.

<p align="center"><img src="../images/readme/ssh-online-terminal.png" width="49%" alt="Bastrio Online-SSH-Terminal" /> <img src="../images/readme/connection-types.png" width="49%" alt="Bastrio Verbindungstypen" /></p>

<p align="center"><img src="../images/readme/remote-workspace.png" width="49%" alt="Bastrio Remote-Arbeitsbereich" /> <img src="../images/readme/sftp-file-browser.png" width="49%" alt="Bastrio SFTP-Dateibrowser" /></p>

<p align="center"><img src="../images/readme/proxy-region-picker.png" width="49%" alt="Bastrio Proxy-Regionsauswahl" /> <img src="../images/readme/split-workspace.png" width="49%" alt="Bastrio geteilter Arbeitsbereich" /></p>

<p align="center"><img src="../images/readme/postgresql-workspace.png" width="49%" alt="Bastrio PostgreSQL-Arbeitsbereich" /> <img src="../images/readme/encrypted-operations-documents.png" width="49%" alt="Bastrio verschlüsselte Arbeitsdokumente" /></p>

<p align="center"><img src="../images/readme/recovery-key.png" width="49%" alt="Bastrio Wiederherstellungsschlüssel" /></p>

## Netzwerkwege unter Ihrer Kontrolle

Mit Bastrio wählen Sie für jeden Browser-Fernzugriff den passenden Weg: eine **Proxy-IP** für die benötigte Ausgangsregion, einen eigenen Proxy für volle Wegkontrolle oder einen **SSH-Jump-Host** für private Infrastruktur. Diese Optionen gehören direkt zur Verbindungseinrichtung.

## Konzentrierte, gemeinsame Remote-Arbeit

Bastrio ist ein Remote-Arbeitsbereich für Entwickler, Betriebsteams und Organisationen, die zwischen Servern, Dateien, Desktops und Datenbanken wechseln. Arbeitsbereiche und geteilte Ressourcen erhalten den Kontext, mehrere Sitzungen und geteilte Ansichten zeigen zusammengehörige Arbeit, und der KI-Assistent bleibt bei der jeweiligen Aufgabe.

## Datenschutz by Design

Anmeldedaten und private Arbeitsbereichsinhalte werden bei der Übertragung und im Ruhezustand verschlüsselt. Bastrio entschlüsselt Anmeldedaten nur vorübergehend im flüchtigen Serverspeicher, wenn sie für eine autorisierte Operation benötigt werden; Klartext wird nie auf Datenträger oder in Logs geschrieben. Jeder nutzerseitig sichtbare Zugriff erfordert eine gültige authentifizierte Sitzung. Nach Ablauf oder Widerruf einer Sitzung kann auf den verschlüsselten Tresor nicht mehr zugegriffen und er nicht mehr entschlüsselt werden. Der Wiederherstellungsschlüssel wird nur einmal angezeigt; er ist nach einer Passwortzurücksetzung zum Wiederherstellen verschlüsselter Anmeldedaten nötig. Ohne ihn kann der verschlüsselte Tresor nicht wiederhergestellt oder lesbar exportiert werden.

## Marketplace, geplant

Bastrio bereitet einen Marketplace für verwaltete Server und Proxy-IP-Dienste vor. Diese Angebote sind für eine spätere Version geplant und derzeit nicht verfügbar.

## Erste Schritte

1. Öffnen Sie [bastr.io](https://bastr.io/), um den Bastrio-Remote-Arbeitsbereich zu starten.
2. Wählen Sie SSH, Dateiübertragung, Remote-Desktop oder eine Datenbankverbindung.
3. Wählen Sie bei Bedarf einen Netzwerkweg und speichern sowie organisieren Sie die Verbindung.

## Häufige Fragen

### Ist Bastrio ein Web-SSH-Terminal?

Ja. Bastrio bietet SSH online im Browser zusammen mit Dateiübertragung, Remote-Desktop, Datenbank-, Proxy- und Arbeitsbereichswerkzeugen.

### Kann ich Proxy-IP, eigenen Proxy und SSH-Jump-Host verwenden?

Ja. Bastrio unterstützt regionale Proxy-IP-Auswahl, eigene Proxy-Konfiguration und SSH-Jump-Hosts.

### Kann ein Team in derselben Umgebung zusammenarbeiten?

Ja. Arbeitsbereiche und geteilte Ressourcen sind dafür konzipiert, Remote-Infrastrukturarbeit geordnet und gemeinschaftlich zu halten.

## Mitwirken

Beiträge und Fehlerberichte sind willkommen. Bitte konzentrieren Sie Vorschläge auf sichtbares Nutzerverhalten und fügen Sie Issues oder Pull Requests keine Anmeldedaten oder privaten Verbindungsdaten bei.

## Lizenz

Bastrio wird unter der [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html) veröffentlicht.
