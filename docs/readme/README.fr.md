<p align="center"><a href="https://bastr.io/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a></p>

<p align="center">Un espace de travail dans le navigateur pour l'accès distant sécurisé, les opérations d'infrastructure et la collaboration.</p>

<p align="center"><a href="https://bastr.io/"><strong>bastr.io</strong></a> &nbsp;|&nbsp; <a href="https://www.gnu.org/licenses/gpl-3.0.html"><img src="https://img.shields.io/badge/license-GPL--3.0--only-2b82f0.svg" alt="GPL-3.0-only" /></a></p>

<p align="center"><a href="../../README.md">English</a> | <a href="README.zh-CN.md">简体中文</a> | <a href="README.zh-TW.md">繁體中文</a> | <a href="README.ja.md">日本語</a> | <a href="README.ko.md">한국어</a> | <a href="README.es.md">Español</a> | <a href="README.de.md">Deutsch</a> | <strong>Français</strong> | <a href="README.pt.md">Português</a> | <a href="README.ar.md">العربية</a></p>

## Un espace de travail pour l'infrastructure distante

[Bastrio](https://bastr.io/) rassemble **SSH online**, SFTP, FTP/FTPS, RDP, VNC et les connexions aux bases de données dans un même espace de travail web. Utilisez-le comme terminal SSH web, gestionnaire de fichiers en ligne, client de base de données dans le navigateur ou espace partagé de gestion de serveurs distants.

![Bastrio SSH online et accès distant dans le navigateur](../images/readme/ssh-online-guest.png)

## Fonctionnalités principales

- **Connexion depuis le navigateur :** terminal SSH en ligne, fichiers SFTP/FTP/FTPS et bureaux distants RDP et VNC.
- **Outils de base de données unifiés :** PostgreSQL, MySQL/MariaDB, SQL Server, Redis et MongoDB dans le même espace de travail.
- **Connexions organisées :** connexions enregistrées, dossiers, filtres par type, récents, sessions multiples et vues fractionnées.
- **Choisissez le chemin réseau :** proxy IP régional, proxy personnalisé ou hôte de rebond SSH pour une infrastructure non exposée directement.
- **Assistance IA :** l'assistant IA aide à expliquer les sorties, préparer des commandes et accompagner le travail de terminal ou de base de données.
- **Espaces collaboratifs :** les espaces de travail et ressources partagées conservent le contexte de connexion de l'équipe.
- **Documents opérationnels chiffrés :** rédigez, chiffrez et conservez notes, brouillons et texte sensible dans l'espace de travail.

<p align="center"><img src="../images/readme/ssh-online-terminal.png" width="49%" alt="Terminal SSH online de Bastrio" /> <img src="../images/readme/connection-types.png" width="49%" alt="Types de connexion Bastrio" /></p>

<p align="center"><img src="../images/readme/remote-workspace.png" width="49%" alt="Espace distant Bastrio" /> <img src="../images/readme/sftp-file-browser.png" width="49%" alt="Navigateur de fichiers SFTP de Bastrio" /></p>

<p align="center"><img src="../images/readme/proxy-region-picker.png" width="49%" alt="Sélecteur de région proxy Bastrio" /> <img src="../images/readme/split-workspace.png" width="49%" alt="Espace de travail fractionné Bastrio" /></p>

<p align="center"><img src="../images/readme/postgresql-workspace.png" width="49%" alt="Espace PostgreSQL Bastrio" /> <img src="../images/readme/encrypted-operations-documents.png" width="49%" alt="Documents opérationnels chiffrés Bastrio" /></p>

<p align="center"><img src="../images/readme/recovery-key.png" width="49%" alt="Clé de récupération Bastrio" /></p>

## Des chemins réseau sous votre contrôle

Bastrio permet de choisir le chemin adapté à chaque accès distant depuis le navigateur : un **proxy IP** pour la région de sortie souhaitée, un proxy personnalisé pour contrôler le trajet, ou un **hôte de rebond SSH** pour atteindre une infrastructure privée. Ces options font partie de la configuration de connexion.

## Un travail distant concentré et collaboratif

Bastrio est un espace de travail distant pour les développeurs, opérateurs et équipes qui passent entre serveurs, fichiers, bureaux et bases de données. Les espaces de travail et ressources partagées préservent le contexte ; les sessions multiples et vues fractionnées gardent le travail lié visible ; l'assistant IA reste à côté de la tâche.

## La confidentialité par conception

Les identifiants et le contenu privé de l'espace de travail sont chiffrés en transit et au repos. Bastrio ne déchiffre les identifiants que temporairement dans la mémoire volatile du serveur lorsqu'une opération autorisée les requiert ; le texte en clair n'est jamais écrit sur disque ni dans les journaux. Chaque accès visible par l'utilisateur exige une session authentifiée valide. Lorsqu'une session expire ou est révoquée, le coffre chiffré ne peut plus être consulté ni déchiffré. La clé de récupération n'est affichée qu'une fois ; elle est nécessaire pour restaurer les identifiants chiffrés après une réinitialisation du mot de passe. Sans elle, le coffre chiffré ne peut pas être restauré ni exporté sous une forme lisible.

## Marketplace, prévu

Bastrio prépare un Marketplace pour des serveurs gérés et des services de proxy IP. Ces offres sont prévues pour une future version et ne sont pas actuellement disponibles.

## Démarrer

1. Visitez [bastr.io](https://bastr.io/) pour ouvrir l'espace de travail distant Bastrio.
2. Choisissez SSH, le transfert de fichiers, le bureau distant ou une connexion à une base de données.
3. Sélectionnez un chemin réseau si nécessaire, puis enregistrez et organisez la connexion.

## Questions fréquentes

### Bastrio est-il un terminal SSH web ?

Oui. Bastrio propose SSH online dans le navigateur avec le transfert de fichiers, le bureau distant, les bases de données, les proxys et les outils d'espace de travail.

### Puis-je utiliser un proxy IP, un proxy personnalisé et un hôte de rebond SSH ?

Oui. Bastrio prend en charge la sélection de proxy IP par région, la configuration de proxy personnalisé et les hôtes de rebond SSH.

### Une équipe peut-elle collaborer dans le même environnement ?

Oui. Les espaces de travail et les ressources partagées sont conçus pour organiser et faciliter la collaboration sur l'infrastructure distante.

## Contribution

Les contributions et signalements de problèmes sont bienvenus. Gardez les propositions centrées sur le comportement visible par l'utilisateur et n'ajoutez pas d'identifiants ni de données de connexion privées aux issues ou pull requests.

## Licence

Bastrio est distribué sous la [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).
