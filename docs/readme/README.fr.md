<p align="center">
  <a href="https://bastr.io/fr/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a>
</p>

# Bastrio — WebSSH, bureaux distants, bases de données et Docker dans votre navigateur

[Bastrio (Bastr.io)](https://bastr.io/fr/) est un espace de travail dans le navigateur pour gérer des serveurs distants. Ouvrez un terminal SSH en ligne, transférez des fichiers par SFTP, accédez à des bureaux RDP ou VNC, travaillez avec des bases de données et gérez des hôtes Docker au même endroit. Les connexions enregistrées, les vues fractionnées, les espaces partagés et l'assistance IA réunissent les tâches liées, avec le stockage chiffré des identifiants et la protection du compte intégrés au travail quotidien.

[Ouvrir l'espace de travail](https://bastr.io/workspace/) · [Lire les guides](../articles/README.md) · [Site web](https://bastr.io/fr/)

[English](../../README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Español](README.es.md) · [Deutsch](README.de.md) · Français · [Português](README.pt.md) · [العربية](README.ar.md)

## Un espace de travail qui suit vos tâches

Partez d'un hôte, ouvrez son terminal, examinez un fichier de configuration, consultez la base de données et vérifiez un conteneur sans devoir reconfigurer vos connexions dans plusieurs applications. Bastrio place les outils à côté du travail : une barre latérale d'hôtes, des onglets de session, des vues fractionnées, des panneaux de fichiers et de bases de données, ainsi que des vues dédiées à Docker et à l'IA.

![Espace de travail Bastrio dans le navigateur avec terminal SSH et gestionnaire de fichiers SFTP en vue fractionnée](../images/readme/split-workspace.png)

| Domaine | Ce que vous pouvez faire depuis l'interface |
| --- | --- |
| Hôtes et sessions | Enregistrer des connexions, les organiser en dossiers, filtrer les types de connexion, rouvrir des sessions récentes et agencer les onglets ou les vues fractionnées. |
| WebSSH et commandes à distance | Utiliser l'authentification SSH par mot de passe ou clé privée, un terminal dans le navigateur, des commandes rapides, la recherche et les commandes de reconnexion. Les types de connexion WinRM et Telnet sont également disponibles lorsqu'ils sont activés. |
| SFTP, FTP et FTPS | Parcourir les répertoires, envoyer et télécharger des fichiers, créer des dossiers, renommer des fichiers et modifier les fichiers texte pris en charge à côté d'un terminal. |
| RDP et VNC | Ouvrir des bureaux distants dans le navigateur, avec des commandes de session, des outils de presse-papiers et des raccourcis clavier. La destination doit disposer d'un service RDP ou VNC accessible. |
| Client de base de données | Se connecter à PostgreSQL, MySQL/MariaDB, SQL Server, Redis et MongoDB. Utiliser l'explorateur de données et les outils de requête, de modification et de sauvegarde disponibles pour le moteur choisi. |
| Docker | Ajouter un hôte SSH existant, découvrir les conteneurs, consulter l'utilisation des ressources et travailler avec les conteneurs, les projets Compose, les images, les volumes et les réseaux. Utiliser les modèles d'applications ou les procédures prises en charge avec des images personnalisées et Compose. |
| Chemins réseau | Choisir une route proxy régionale disponible, configurer votre propre proxy ou utiliser un hôte de rebond SSH. |
| Espaces de travail partagés | Passer d'un espace personnel à un espace d'équipe, inviter des membres et accorder l'accès à certaines ressources. |
| IA et MCP | Demander de l'aide pendant le travail dans un terminal ou une base de données, ou connecter un client MCP aux ressources que vous autorisez. |
| Runbooks chiffrés et stockage cloud | Organiser les documents de travail, chiffrer les runbooks sensibles avec un mot de passe distinct et gérer les fichiers dans le stockage dont vous disposez. |

Les protocoles disponibles, les actions Docker, les écritures dans les bases de données, l'utilisation de l'IA et le stockage dépendent de votre compte, des autorisations de l'espace de travail et du service connecté. L'interface actuelle indique ce qui est disponible pour votre session.

## Le chiffrement et les accès sous votre contrôle

Bastrio associe le stockage chiffré à des paramètres visibles de protection du compte et des connexions :

- **Identifiants de connexion chiffrés.** Les mots de passe de connexion et les clés privées enregistrés sont protégés au repos par AES-256-GCM.
- **Transport protégé.** Utilisez Bastr.io en HTTPS. SSH/SFTP et FTPS assurent un transport chiffré vers le système distant ; choisissez un protocole sécurisé adapté à la destination.
- **Protection du compte.** Activez l'authentification à deux facteurs et conservez votre clé de récupération hors ligne. La procédure de récupération aide à rétablir l'accès aux identifiants de connexion chiffrés après une réinitialisation du mot de passe.
- **Runbooks chiffrés.** Choisissez le mode chiffré et un mot de passe de document distinct pour les notes sensibles. Confirmez le chiffrement et l'enregistrement dans l'éditeur et conservez le mot de passe du document en lieu sûr.
- **Accès IA contrôlé.** Les clés d'API MCP disposent d'autorisations sélectionnées et de paramètres d'expiration et de révocation. Examinez les demandes d'approbation dans le navigateur avant d'autoriser des opérations sensibles et gérez les identifiants des serveurs depuis l'interface de l'espace de travail.

Ces protections complètent les autorisations et les mesures de sécurité de vos systèmes distants. Gardez les éléments de récupération et les véritables identifiants hors des documents partagés, des captures d'écran et des conversations avec l'IA.

## Alternatives pour WebSSH, les bases de données et Docker

Bastrio est utile lorsque votre besoin principal est un travail partagé dans le navigateur sur plusieurs types de ressources distantes. Si vous cherchez une alternative à Termius, une alternative dans le navigateur à FinalShell ou Xshell, un client de base de données de type Navicat ou une alternative à Portainer pour Docker via SSH, partez de la tâche à accomplir.

| Outils que vous comparez peut-être | Quand envisager Bastrio | Guide détaillé |
| --- | --- | --- |
| Termius, FinalShell, MobaXterm, Xshell, SecureCRT et PuTTY | Vous voulez SSH dans le navigateur, des hôtes enregistrés, des sessions fractionnées et des outils de fichiers à proximité. Vérifiez séparément les besoins en scripts de bureau ou en X11. | [Outils SSH et espaces de travail dans le navigateur](../articles/fr/ssh-tools-browser-workspace.md) |
| WinSCP, FileZilla, Xftp et Cyberduck | Vous voulez transférer des fichiers par SFTP ou FTP/FTPS et modifier du texte à côté de votre session distante. | [Outils et méthodes de travail FTP/SFTP](../articles/fr/ftp-sftp-tools-browser-workflow.md) |
| Navicat, DBeaver, DataGrip, pgAdmin, Redis Insight et MongoDB Compass | Vous voulez un client de base de données dans le navigateur à côté de vos hôtes. Choisissez selon le moteur et vos besoins en requêtes, modifications et sauvegardes. | [Outils pour les bases de données distantes](../articles/fr/remote-database-tools-comparison.md) |
| Apache Guacamole, TeamViewer, AnyDesk et ToDesk | Vous avez besoin d'accéder depuis le navigateur à une destination RDP/VNC existante. L'assistance à distance en présence d'un utilisateur et les passerelles de bureau ont des exigences de connexion différentes. | [Bureaux distants dans le navigateur](../articles/fr/browser-remote-desktop-tools.md) |
| Portainer, Dockge et Docker Desktop | Vous voulez gérer des ressources Docker et Compose distantes via un hôte SSH existant. Le développement local de conteneurs et l'administration de clusters constituent des critères de choix distincts. | [Gestion de Docker selon le scénario](../articles/fr/docker-management-tools-by-scenario.md) |
| Méthodes de travail MCP avec des outils SSH, de base de données et Docker | Vous voulez qu'un client IA découvre et utilise les ressources autorisées avec des permissions et des contrôles d'approbation. | [Gestion à distance avec MCP](../articles/fr/mcp-remote-management-tools.md) |

Ces comparaisons portent sur les méthodes de travail. Les fonctionnalités varient selon le produit, l'édition et la configuration ; les guides liés expliquent dans quels cas un outil spécialisé peut mieux convenir.

## Démarrer dans le navigateur

1. Visitez [bastr.io](https://bastr.io/fr/). Utilisez une connexion invitée disponible pour une session temporaire, ou connectez-vous pour enregistrer et organiser votre travail.
2. Choisissez un type de connexion et saisissez la destination dans **Quick Connect**, ou ajoutez-la sous **Hosts**. Saisissez les mots de passe et les clés privées uniquement dans le formulaire de connexion.
3. Sélectionnez un proxy ou un hôte de rebond SSH si la destination nécessite un chemin réseau particulier.
4. Ouvrez la session. Utilisez **Files**, le panneau de base de données ou **Docker** pour la tâche suivante et agencez les sessions liées avec les commandes de disposition.
5. Pour le travail en équipe, sélectionnez le bon espace de travail et partagez les ressources dont les membres ont besoin. Activez l'authentification à deux facteurs et sauvegardez les éléments de récupération avant de compter sur ce compte pour les accès quotidiens.

L'accès invité a ses propres conditions de disponibilité et limites d'utilisation. Les hôtes enregistrés, les fonctions d'équipe et certains outils nécessitent une connexion au compte ou un compte éligible.

## Gérer Docker via SSH

Ouvrez **Docker** dans l'espace de travail et sélectionnez un hôte SSH auquel vous avez accès. La vue Docker réunit les conteneurs, Compose, les images, les volumes, les réseaux et la progression des tâches. Vous pouvez examiner l'état des conteneurs et leur utilisation des ressources, effectuer les actions de cycle de vie prises en charge et lancer un déploiement à partir des modèles d'applications disponibles, d'une image personnalisée ou d'une configuration Compose prise en charge.

Si Docker est absent, l'interface peut vous guider dans son installation sur les hôtes Linux pris en charge, après examen et confirmation de l'action proposée. La disponibilité dépend de l'hôte, de vos autorisations et des fonctionnalités auxquelles vous avez actuellement accès. Consultez le [guide comparatif Docker](../articles/fr/docker-management-tools-by-scenario.md) pour une démarche d'évaluation pratique.

## Connecter des clients IA avec MCP

Bastrio prend en charge les connexions Model Context Protocol (MCP) depuis des clients tels que Claude Code, Codex, Cursor et VS Code. MCP complète l'assistant IA intégré : il permet au client de votre choix de travailler avec les hôtes, fichiers, bases de données et chemins réseau autorisés.

1. Ouvrez **Tools → MCP API Keys** dans l'espace de travail.
2. Créez une clé avec les autorisations et la durée de validité dont votre client a besoin.
3. Sélectionnez le client et suivez les instructions de connexion affichées sur cette page.
4. Conservez la clé dans la configuration de secrets ou d'environnement prise en charge par le client. Examinez les demandes d'approbation dans le navigateur et révoquez l'accès lorsqu'il n'est plus nécessaire.

Utilisez le point de terminaison indiqué dans votre compte. Les outils disponibles dépendent des autorisations accordées ; le client doit les découvrir auprès du service MCP. Le [guide MCP](../articles/fr/mcp-remote-management-tools.md) donne des exemples d'utilisation avec SSH, les bases de données et Docker.

## Six guides pratiques en dix langues

La [bibliothèque de guides](../articles/README.md) contient les six comparatifs publiés en anglais, chinois simplifié, chinois traditionnel, espagnol, allemand, français, japonais, coréen, malais et russe. Chaque version conserve le texte existant des articles, les illustrations, les questions fréquentes et un lien vers la page Bastr.io d'origine.

[English guides](../articles/en/README.md) · [简体中文指南](../articles/zh/README.md) · [繁體中文指南](../articles/zh-TW/README.md) · [日本語](../articles/ja/README.md) · [한국어](../articles/ko/README.md) · [Español](../articles/es/README.md) · [Deutsch](../articles/de/README.md) · [Français](../articles/fr/README.md) · [Bahasa Melayu](../articles/ms/README.md) · [Русский](../articles/ru/README.md)

## Questions fréquentes

### Qu'est-ce que Bastrio ?

Bastrio est un espace de travail dans le navigateur qui réunit WebSSH, le transfert de fichiers, RDP/VNC, les bases de données, la gestion de Docker, les ressources partagées et l'assistance IA. Il est conçu pour les développeurs et les équipes d'exploitation qui travaillent sur plusieurs systèmes distants.

### Bastrio peut-il remplacer Termius, FinalShell ou MobaXterm ?

Bastrio propose une méthode de travail dans le navigateur pour les tâches courantes de SSH et de gestion de fichiers. Avant de changer d'outil, évaluez les fonctions de bureau dont vous dépendez, comme l'intégration du shell local, les macros ou X11. Le [comparatif SSH](../articles/fr/ssh-tools-browser-workspace.md) vous aide à choisir selon le scénario.

### Bastrio est-il une alternative à Navicat ou DBeaver dans le navigateur ?

Il peut couvrir les usages courants de bases de données distantes PostgreSQL, MySQL/MariaDB, SQL Server, Redis et MongoDB. Les opérations disponibles varient selon le moteur et les autorisations. La modélisation avancée, la synchronisation et les processus de développement spécialisés doivent être évalués au regard de vos besoins.

### Bastrio est-il une alternative à Portainer ?

Pour les utilisateurs qui souhaitent gérer des hôtes Docker et Compose à côté de SSH, des fichiers et des bases de données, Bastrio propose une méthode de travail dans le navigateur via une connexion SSH existante. Comparez le [guide Docker](../articles/fr/docker-management-tools-by-scenario.md) avec votre environnement et vos besoins de déploiement.

### Dois-je installer un client de bureau ?

Vous pouvez utiliser l'espace de travail depuis un navigateur pris en charge. La destination doit toujours disposer d'un service SSH, de transfert de fichiers, de bureau distant ou de base de données accessible, ainsi que d'identifiants d'accès valides.

### Comment les identifiants de connexion et les notes sensibles sont-ils protégés ?

Les identifiants de connexion enregistrés sont chiffrés au repos avec AES-256-GCM, et Bastr.io utilise HTTPS pour l'accès depuis le navigateur. Les runbooks sensibles peuvent être enregistrés sous forme chiffrée avec un mot de passe de document distinct. L'authentification à deux facteurs, les éléments de récupération et les autorisations sur les ressources apportent des contrôles supplémentaires.

### Puis-je commencer sans compte ?

Utilisez une connexion invitée lorsque la page d'accueil la propose. L'accès invité, les protocoles et les durées autorisées peuvent changer ; connectez-vous pour retrouver les connexions enregistrées et les outils disponibles pour votre compte.

## Contact et informations sur le projet

Site web : [bastr.io](https://bastr.io/fr/) · Assistance : [sup@bastr.io](mailto:sup@bastr.io) · [Signaler un problème](https://github.com/cihalqe/bastrio/issues)

Ce dépôt contient la documentation publique du produit Bastrio et ses guides. Les suggestions et les corrections sont les bienvenues. Partagez uniquement des exemples sans données sensibles dans les issues et les pull requests.

Licence : [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).
