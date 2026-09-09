<p align="center">
  <a href="https://bastr.io/de/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a>
</p>

# Bastrio — WebSSH, Remote-Desktops, Datenbanken und Docker im Browser

[Bastrio (Bastr.io)](https://bastr.io/de/) ist ein Browser-Arbeitsbereich für die Verwaltung entfernter Server. Öffnen Sie ein Online-SSH-Terminal, übertragen Sie Dateien per SFTP, verbinden Sie sich mit RDP- oder VNC-Desktops, arbeiten Sie mit Datenbanken und verwalten Sie Docker-Hosts an einem Ort. Gespeicherte Verbindungen, geteilte Ansichten, gemeinsame Arbeitsbereiche und KI-Unterstützung halten zusammengehörige Aufgaben beieinander. Verschlüsselte Anmeldedaten und Kontoschutz sind dabei Teil des Arbeitsablaufs.

[Arbeitsbereich öffnen](https://bastr.io/workspace/) · [Anleitungen lesen](../articles/README.md) · [Website](https://bastr.io/de/)

[English](../../README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Español](README.es.md) · Deutsch · [Français](README.fr.md) · [Português](README.pt.md) · [العربية](README.ar.md)

## Ein Arbeitsbereich, der Ihre Aufgaben begleitet

Beginnen Sie bei einem Host, öffnen Sie sein Terminal, prüfen Sie eine Konfigurationsdatei, sehen Sie in der Datenbank nach und überprüfen Sie einen Container, ohne Ihre Verbindungen in mehreren Anwendungen erneut einrichten zu müssen. Bastrio bringt die Werkzeuge direkt zur Aufgabe: eine Host-Seitenleiste, Sitzungsregisterkarten, geteilte Ansichten, Datei- und Datenbankbereiche sowie eigene Ansichten für Docker und KI.

![Bastrio-Browser-Arbeitsbereich mit SSH-Terminal und SFTP-Dateimanager in einer geteilten Ansicht](../images/readme/split-workspace.png)

| Bereich | Möglichkeiten in der Benutzeroberfläche |
| --- | --- |
| Hosts und Sitzungen | Verbindungen speichern, in Ordnern organisieren, nach Verbindungstyp filtern, letzte Sitzungen erneut öffnen und Registerkarten oder geteilte Ansichten anordnen. |
| WebSSH und Remote-Befehle | SSH mit Passwort oder privatem Schlüssel, ein Browser-Terminal, Schnellbefehle, Suche und Steuerelemente zum Wiederverbinden nutzen. WinRM und Telnet stehen ebenfalls als Verbindungstypen zur Verfügung, sofern sie freigeschaltet sind. |
| SFTP, FTP und FTPS | Verzeichnisse durchsuchen, Dateien hoch- und herunterladen, Ordner erstellen, Dateien umbenennen und unterstützte Textdateien neben dem Terminal bearbeiten. |
| RDP und VNC | Remote-Desktops im Browser öffnen, mit Sitzungssteuerung, Zwischenablage und Tastenkombinationen. Das Ziel benötigt einen erreichbaren RDP- oder VNC-Dienst. |
| Datenbankclient | Verbindungen zu PostgreSQL, MySQL/MariaDB, SQL Server, Redis und MongoDB herstellen. Den Datenbrowser und die verfügbaren Abfrage-, Bearbeitungs- und Sicherungswerkzeuge des jeweiligen Datenbanksystems nutzen. |
| Docker | Einen vorhandenen SSH-Host hinzufügen, Container erkennen, die Ressourcennutzung anzeigen und mit Containern, Compose-Projekten, Images, Volumes und Netzwerken arbeiten. Anwendungsvorlagen oder unterstützte Abläufe mit eigenen Images und Compose verwenden. |
| Netzwerkwege | Eine verfügbare regionale Proxy-Route wählen, einen eigenen Proxy konfigurieren oder einen SSH-Jump-Host verwenden. |
| Gemeinsame Arbeitsbereiche | Zwischen persönlichen und Team-Arbeitsbereichen wechseln, Mitglieder einladen und Zugriff auf ausgewählte Ressourcen gewähren. |
| KI und MCP | Unterstützung direkt bei der Terminal- oder Datenbankarbeit erhalten oder einen MCP-Client mit den Ressourcen verbinden, die Sie freigeben. |
| Verschlüsselte Runbooks und Cloud-Speicher | Arbeitsdokumente organisieren, sensible Runbooks mit einem separaten Passwort verschlüsseln und Dateien im verfügbaren Speicher verwalten. |

Verfügbare Protokolle, Docker-Aktionen, Schreibzugriffe auf Datenbanken, KI-Nutzung und Speicher hängen von Ihrem Konto, den Berechtigungen im Arbeitsbereich und dem verbundenen Dienst ab. Die aktuelle Oberfläche zeigt, was für Ihre Sitzung verfügbar ist.

## Verschlüsselung und Zugriff unter Ihrer Kontrolle

Bastrio verbindet verschlüsselte Speicherung mit sichtbaren Schutz- und Zugriffseinstellungen für Konto und Verbindungen:

- **Verschlüsselte Zugangsdaten.** Gespeicherte Verbindungspasswörter und private Schlüssel werden im Ruhezustand mit AES-256-GCM geschützt.
- **Geschützte Übertragung.** Verwenden Sie Bastr.io über HTTPS. SSH/SFTP und FTPS bieten eine verschlüsselte Übertragung zum entfernten System; wählen Sie ein sicheres Protokoll, das zum Ziel passt.
- **Kontoschutz.** Aktivieren Sie die Zwei-Faktor-Authentifizierung und bewahren Sie Ihren Wiederherstellungsschlüssel offline auf. Der Wiederherstellungsablauf hilft, nach einer Passwortzurücksetzung den Zugriff auf verschlüsselte Zugangsdaten wiederherzustellen.
- **Verschlüsselte Runbooks.** Wählen Sie für sensible Notizen den verschlüsselten Modus und ein separates Dokumentpasswort. Bestätigen Sie Verschlüsselung und Speicherung im Editor und bewahren Sie das Dokumentpasswort sicher auf.
- **Kontrollierter KI-Zugriff.** MCP-API-Schlüssel verfügen über ausgewählte Berechtigungen, ein Ablaufdatum und Möglichkeiten zum Widerruf. Prüfen Sie Freigabeanfragen im Browser, bevor Sie sensible Aktionen erlauben, und verwalten Sie Server-Anmeldedaten über die Oberfläche des Arbeitsbereichs.

Diese Schutzmaßnahmen ergänzen die Berechtigungen und Sicherheitsvorkehrungen Ihrer entfernten Systeme. Bewahren Sie Wiederherstellungsdaten und echte Anmeldedaten außerhalb gemeinsam genutzter Dokumente, Screenshots und KI-Unterhaltungen auf.

## Alternativen für WebSSH, Datenbanken und Docker

Bastrio eignet sich, wenn Sie vor allem einen gemeinsamen Browser-Arbeitsablauf für verschiedene Arten entfernter Ressourcen benötigen. Ob Sie eine Termius-Alternative, eine Browser-Alternative zu FinalShell oder Xshell, einen Datenbankclient ähnlich Navicat oder eine Portainer-Alternative für Docker über SSH vergleichen: Beginnen Sie bei der Aufgabe, die Sie erledigen möchten.

| Mögliche Vergleichswerkzeuge | Wann Bastrio infrage kommt | Ausführliche Anleitung |
| --- | --- | --- |
| Termius, FinalShell, MobaXterm, Xshell, SecureCRT und PuTTY | Sie möchten SSH im Browser, gespeicherte Hosts, geteilte Sitzungen und Dateiverwaltung direkt daneben. Prüfen Sie Anforderungen an Desktop-Skripte oder X11 gesondert. | [SSH-Werkzeuge und Browser-Arbeitsbereiche](../articles/de/ssh-tools-browser-workspace.md) |
| WinSCP, FileZilla, Xftp und Cyberduck | Sie möchten Dateien per SFTP oder FTP/FTPS übertragen und Texte neben Ihrer Remote-Sitzung bearbeiten. | [FTP/SFTP-Werkzeuge und Arbeitsabläufe](../articles/de/ftp-sftp-tools-browser-workflow.md) |
| Navicat, DBeaver, DataGrip, pgAdmin, Redis Insight und MongoDB Compass | Sie möchten einen Datenbankclient im Browser direkt neben Ihren Hosts. Entscheiden Sie nach Datenbanksystem sowie Abfrage-, Bearbeitungs- und Sicherungsbedarf. | [Werkzeuge für entfernte Datenbanken](../articles/de/remote-database-tools-comparison.md) |
| Apache Guacamole, TeamViewer, AnyDesk und ToDesk | Sie benötigen Browser-Zugriff auf ein vorhandenes RDP/VNC-Ziel. Fernunterstützung mit anwesenden Nutzern und Desktop-Gateways haben andere Verbindungsanforderungen. | [Remote-Desktops im Browser](../articles/de/browser-remote-desktop-tools.md) |
| Portainer, Dockge und Docker Desktop | Sie möchten entfernte Docker- und Compose-Ressourcen über einen vorhandenen SSH-Host verwalten. Lokale Container-Entwicklung und Cluster-Verwaltung sind eigene Auswahlkriterien. | [Docker-Verwaltung nach Einsatzbereich](../articles/de/docker-management-tools-by-scenario.md) |
| MCP-Arbeitsabläufe neben SSH-, Datenbank- und Docker-Werkzeugen | Sie möchten, dass ein KI-Client freigegebene Ressourcen mit Berechtigungen und Freigabekontrollen erkennen und bedienen kann. | [Remote-Verwaltung mit MCP](../articles/de/mcp-remote-management-tools.md) |

Diese Vergleiche beziehen sich auf Arbeitsabläufe. Der Funktionsumfang hängt von Produkt, Edition und Konfiguration ab; die verlinkten Anleitungen erläutern, wann ein spezialisiertes Werkzeug besser passen kann.

## Im Browser loslegen

1. Öffnen Sie [bastr.io](https://bastr.io/de/). Verwenden Sie eine verfügbare Gastverbindung für eine vorübergehende Sitzung oder melden Sie sich an, um Ihre Arbeit zu speichern und zu organisieren.
2. Wählen Sie einen Verbindungstyp und geben Sie das Ziel unter **Quick Connect** ein oder fügen Sie es unter **Hosts** hinzu. Geben Sie Passwörter und private Schlüssel ausschließlich in das Verbindungsformular ein.
3. Wählen Sie einen Proxy oder SSH-Jump-Host, falls das Ziel einen bestimmten Netzwerkweg benötigt.
4. Öffnen Sie die Sitzung. Nutzen Sie **Files**, den Datenbankbereich oder **Docker** für die nächste Aufgabe und ordnen Sie zusammengehörige Sitzungen mit den Layout-Steuerelementen an.
5. Wählen Sie für die Teamarbeit den richtigen Arbeitsbereich und teilen Sie die benötigten Ressourcen mit den Mitgliedern. Aktivieren Sie die Zwei-Faktor-Authentifizierung und sichern Sie Ihre Wiederherstellungsdaten, bevor Sie das Konto für den täglichen Zugriff einsetzen.

Für den Gastzugang gelten eigene Verfügbarkeiten und Nutzungslimits. Gespeicherte Hosts, Teamfunktionen und einige Werkzeuge erfordern eine Anmeldung oder ein entsprechend berechtigtes Konto.

## Docker über SSH verwalten

Öffnen Sie **Docker** im Arbeitsbereich und wählen Sie einen SSH-Host, auf den Sie zugreifen können. Die Docker-Ansicht vereint Container, Compose, Images, Volumes, Netzwerke und den Aufgabenfortschritt. Sie können Containerzustand und Ressourcennutzung prüfen, unterstützte Aktionen im Container-Lebenszyklus ausführen und eine Bereitstellung aus den verfügbaren Anwendungsvorlagen, einem eigenen Image oder einer unterstützten Compose-Konfiguration starten.

Falls Docker fehlt, kann die Oberfläche auf unterstützten Linux-Hosts durch die Installation führen, nachdem Sie die vorgeschlagene Aktion geprüft und bestätigt haben. Die Verfügbarkeit hängt vom Host, Ihren Berechtigungen und den aktuell freigeschalteten Funktionen ab. Die [Docker-Vergleichsanleitung](../articles/de/docker-management-tools-by-scenario.md) zeigt einen praktischen Ablauf zur Bewertung.

## KI-Clients über MCP verbinden

Bastrio unterstützt Verbindungen über das Model Context Protocol (MCP) von Clients wie Claude Code, Codex, Cursor und VS Code. MCP ergänzt den integrierten KI-Assistenten: Ihr gewählter Client kann damit mit freigegebenen Hosts, Dateien, Datenbanken und Netzwerkwegen arbeiten.

1. Öffnen Sie **Tools → MCP API Keys** im Arbeitsbereich.
2. Erstellen Sie einen Schlüssel mit den Berechtigungen und der Gültigkeitsdauer, die Ihr Client benötigt.
3. Wählen Sie den Client und verwenden Sie die auf dieser Seite angezeigte Verbindungsanleitung.
4. Bewahren Sie den Schlüssel in der vom Client unterstützten Konfiguration für Geheimnisse oder Umgebungsvariablen auf. Prüfen Sie Freigabeanfragen im Browser und widerrufen Sie den Zugriff, wenn er nicht mehr benötigt wird.

Verwenden Sie den in Ihrem Konto angezeigten Endpunkt. Die verfügbaren Werkzeuge hängen von den erteilten Berechtigungen ab; der Client sollte sie über den MCP-Dienst ermitteln. Die [MCP-Anleitung](../articles/de/mcp-remote-management-tools.md) zeigt Beispiele für das Zusammenspiel mit SSH-, Datenbank- und Docker-Aufgaben.

## Sechs praktische Anleitungen in zehn Sprachen

Die [Anleitungsbibliothek](../articles/README.md) enthält die sechs veröffentlichten Vergleiche auf Englisch, vereinfachtem Chinesisch, traditionellem Chinesisch, Spanisch, Deutsch, Französisch, Japanisch, Koreanisch, Malaiisch und Russisch. Jede Fassung bewahrt den bestehenden Artikeltext, die Abbildungen, die häufigen Fragen und einen Link zur ursprünglichen Bastr.io-Seite.

[English guides](../articles/en/README.md) · [简体中文指南](../articles/zh/README.md) · [繁體中文指南](../articles/zh-TW/README.md) · [日本語](../articles/ja/README.md) · [한국어](../articles/ko/README.md) · [Español](../articles/es/README.md) · [Deutsch](../articles/de/README.md) · [Français](../articles/fr/README.md) · [Bahasa Melayu](../articles/ms/README.md) · [Русский](../articles/ru/README.md)

## Häufige Fragen

### Was ist Bastrio?

Bastrio ist ein Browser-Arbeitsbereich, der WebSSH, Dateiübertragung, RDP/VNC, Datenbanken, Docker-Verwaltung, geteilte Ressourcen und KI-Unterstützung verbindet. Er richtet sich an Entwickler und Betriebsteams, die mit mehreren entfernten Systemen arbeiten.

### Kann Bastrio Termius, FinalShell oder MobaXterm ersetzen?

Bastrio bietet einen Browser-Arbeitsablauf für gängige SSH- und Dateiverwaltungsaufgaben. Prüfen Sie vor einem Wechsel die Desktop-Funktionen, auf die Sie angewiesen sind, etwa die Einbindung einer lokalen Shell, Makros oder X11. Der [SSH-Vergleich](../articles/de/ssh-tools-browser-workspace.md) hilft Ihnen, nach Einsatzbereich zu entscheiden.

### Ist Bastrio eine Browser-Alternative zu Navicat oder DBeaver?

Es kann gängige Arbeitsabläufe mit entfernten PostgreSQL-, MySQL/MariaDB-, SQL-Server-, Redis- und MongoDB-Datenbanken abdecken. Die verfügbaren Aktionen unterscheiden sich je nach Datenbanksystem und Berechtigungen. Erweiterte Modellierung, Synchronisierung und spezialisierte Entwicklungsabläufe sollten Sie anhand Ihrer Anforderungen bewerten.

### Ist Bastrio eine Portainer-Alternative?

Wenn Sie Docker-Hosts und Compose neben SSH, Dateien und Datenbanken verwalten möchten, bietet Bastrio einen Browser-Arbeitsablauf über eine vorhandene SSH-Verbindung. Gleichen Sie die [Docker-Anleitung](../articles/de/docker-management-tools-by-scenario.md) mit Ihrer Umgebung und Ihren Bereitstellungsanforderungen ab.

### Muss ich einen Desktop-Client installieren?

Sie können den Arbeitsbereich in einem unterstützten Browser nutzen. Das Ziel benötigt weiterhin einen erreichbaren SSH-, Dateiübertragungs-, Remote-Desktop- oder Datenbankdienst und gültige Zugangsdaten.

### Wie werden Zugangsdaten und sensible Notizen geschützt?

Gespeicherte Zugangsdaten werden im Ruhezustand mit AES-256-GCM verschlüsselt, und Bastr.io verwendet HTTPS für den Browser-Zugriff. Sensible Runbooks lassen sich mit einem separaten Dokumentpasswort verschlüsselt speichern. Zwei-Faktor-Authentifizierung, Wiederherstellungsdaten und Ressourcenberechtigungen bieten zusätzliche Kontrollmöglichkeiten.

### Kann ich ohne Konto starten?

Nutzen Sie eine Gastverbindung, wenn diese auf der Startseite angeboten wird. Gastzugang, Protokolle und Zeitlimits können sich ändern; melden Sie sich an, um gespeicherte Verbindungen und die für Ihr Konto verfügbaren Werkzeuge zu nutzen.

## Kontakt und Projektinformationen

Website: [bastr.io](https://bastr.io/de/) · Support: [sup@bastr.io](mailto:sup@bastr.io) · [Problem melden](https://github.com/cihalqe/bastrio/issues)

Dieses Repository enthält die öffentliche Produktdokumentation und Anleitungen von Bastrio. Vorschläge und Korrekturen sind willkommen. Teilen Sie in Issues und Pull Requests nur Beispiele ohne sensible Daten.

Lizenz: [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).
