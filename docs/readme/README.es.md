<p align="center">
  <a href="https://bastr.io/es/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a>
</p>

# Bastrio — WebSSH, escritorios remotos, bases de datos y Docker en tu navegador

[Bastrio (Bastr.io)](https://bastr.io/es/) es un espacio de trabajo en el navegador para gestionar servidores remotos. Abre una terminal SSH en línea, transfiere archivos por SFTP, conéctate a escritorios RDP o VNC, trabaja con bases de datos y administra hosts Docker en un solo lugar. Las conexiones guardadas, las vistas divididas, los espacios compartidos y la asistencia con IA reúnen las tareas relacionadas, con almacenamiento cifrado de credenciales y protección de la cuenta integrados en el flujo de trabajo.

[Abrir el espacio de trabajo](https://bastr.io/workspace/) · [Leer las guías](../articles/README.md) · [Sitio web](https://bastr.io/es/)

[English](../../README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · Español · [Deutsch](README.de.md) · [Français](README.fr.md) · [Português](README.pt.md) · [العربية](README.ar.md)

## Un espacio de trabajo que acompaña tus tareas

Empieza por un host, abre su terminal, revisa un archivo de configuración, consulta la base de datos e inspecciona un contenedor sin tener que configurar de nuevo tus conexiones en varias aplicaciones. Bastrio sitúa las herramientas junto al trabajo: una barra lateral de hosts, pestañas de sesión, vistas divididas, paneles de archivos y bases de datos, y vistas específicas de Docker e IA.

![Espacio de trabajo de Bastrio en el navegador con terminal SSH y gestor de archivos SFTP en una vista dividida](../images/readme/split-workspace.png)

| Área | Qué puedes hacer desde la interfaz |
| --- | --- |
| Hosts y sesiones | Guardar conexiones, organizarlas en carpetas, filtrar por tipo de conexión, reabrir sesiones recientes y distribuir pestañas o vistas divididas. |
| WebSSH y comandos remotos | Usar autenticación SSH con contraseña o clave privada, una terminal en el navegador, comandos rápidos, búsqueda y controles de reconexión. Los tipos de conexión WinRM y Telnet también están disponibles cuando están habilitados. |
| SFTP, FTP y FTPS | Explorar directorios, subir y descargar archivos, crear carpetas, renombrar archivos y editar los archivos de texto compatibles junto a una terminal. |
| RDP y VNC | Abrir escritorios remotos en el navegador, con controles de sesión, herramientas del portapapeles y atajos de teclado. El destino necesita un servicio RDP o VNC accesible. |
| Cliente de bases de datos | Conectarte a PostgreSQL, MySQL/MariaDB, SQL Server, Redis y MongoDB. Usar el explorador de datos y las herramientas de consulta, edición y copia de seguridad disponibles para cada motor. |
| Docker | Añadir un host SSH existente, descubrir contenedores, consultar el uso de recursos y trabajar con contenedores, proyectos Compose, imágenes, volúmenes y redes. Usar plantillas de aplicaciones o flujos compatibles con imágenes personalizadas y Compose. |
| Rutas de red | Elegir una ruta de proxy regional disponible, configurar tu propio proxy o usar un host de salto SSH. |
| Espacios de trabajo compartidos | Cambiar entre espacios personales y de equipo, invitar a miembros y conceder acceso a recursos seleccionados. |
| IA y MCP | Pedir ayuda junto al trabajo en la terminal o la base de datos, o conectar un cliente MCP a los recursos que autorices. |
| Runbooks cifrados y almacenamiento en la nube | Organizar documentos de trabajo, cifrar runbooks sensibles con una contraseña independiente y gestionar archivos en el almacenamiento disponible. |

Los protocolos disponibles, las acciones de Docker, las escrituras en bases de datos, el uso de IA y el almacenamiento dependen de tu cuenta, los permisos del espacio de trabajo y el servicio conectado. La interfaz actual muestra qué está disponible para tu sesión.

## Cifrado y acceso bajo tu control

Bastrio combina el almacenamiento cifrado con controles visibles de protección de la cuenta y las conexiones:

- **Credenciales de conexión cifradas.** Las contraseñas de conexión y las claves privadas guardadas están protegidas en reposo con AES-256-GCM.
- **Transporte protegido.** Usa Bastr.io a través de HTTPS. SSH/SFTP y FTPS ofrecen transporte remoto cifrado; elige un protocolo seguro adecuado para el destino.
- **Protección de la cuenta.** Activa la autenticación de dos factores y conserva tu clave de recuperación sin conexión. El proceso de recuperación ayuda a recuperar el acceso a las credenciales de conexión cifradas tras restablecer la contraseña.
- **Runbooks cifrados.** Elige el modo cifrado y una contraseña de documento independiente para las notas sensibles. Confirma el cifrado y el guardado en el editor, y conserva la contraseña del documento en un lugar seguro.
- **Acceso controlado para la IA.** Las claves de API de MCP tienen permisos seleccionados y controles de caducidad y revocación. Revisa las solicitudes de aprobación en el navegador antes de permitir operaciones sensibles y gestiona las credenciales de los servidores desde la interfaz del espacio de trabajo.

Estas protecciones complementan los permisos y la seguridad de tus sistemas remotos. Mantén el material de recuperación y las credenciales reales fuera de los documentos compartidos, las capturas de pantalla y las conversaciones con IA.

## Alternativas para WebSSH, bases de datos y Docker

Bastrio resulta útil cuando tu necesidad principal es un flujo de trabajo compartido en el navegador para varios tipos de recursos remotos. Si comparas una alternativa a Termius, una alternativa en el navegador a FinalShell o Xshell, un cliente de bases de datos similar a Navicat o una alternativa a Portainer para Docker por SSH, empieza por la tarea que necesitas completar.

| Herramientas que quizá estés comparando | Cuándo considerar Bastrio | Guía detallada |
| --- | --- | --- |
| Termius, FinalShell, MobaXterm, Xshell, SecureCRT y PuTTY | Quieres SSH en el navegador, hosts guardados, sesiones divididas y herramientas de archivos al lado. Comprueba por separado los requisitos de scripts de escritorio o X11. | [Herramientas SSH y espacios de trabajo en el navegador](../articles/es/ssh-tools-browser-workspace.md) |
| WinSCP, FileZilla, Xftp y Cyberduck | Quieres transferencias SFTP o FTP/FTPS y edición de texto junto a tu sesión remota. | [Herramientas y flujos de trabajo FTP/SFTP](../articles/es/ftp-sftp-tools-browser-workflow.md) |
| Navicat, DBeaver, DataGrip, pgAdmin, Redis Insight y MongoDB Compass | Quieres un cliente de bases de datos en el navegador junto a tus hosts. Elige según el motor y tus necesidades de consulta, edición y copia de seguridad. | [Herramientas para bases de datos remotas](../articles/es/remote-database-tools-comparison.md) |
| Apache Guacamole, TeamViewer, AnyDesk y ToDesk | Necesitas acceso desde el navegador a un destino RDP/VNC existente. La asistencia remota con un usuario presente y las pasarelas de escritorio tienen requisitos de conexión diferentes. | [Escritorios remotos en el navegador](../articles/es/browser-remote-desktop-tools.md) |
| Portainer, Dockge y Docker Desktop | Quieres gestionar recursos remotos de Docker y Compose a través de un host SSH existente. El desarrollo local con contenedores y la administración de clústeres son criterios de selección distintos. | [Gestión de Docker según el escenario](../articles/es/docker-management-tools-by-scenario.md) |
| Flujos de trabajo MCP junto a herramientas de SSH, bases de datos y Docker | Quieres que un cliente de IA descubra y opere recursos autorizados con permisos y controles de aprobación. | [Gestión remota con MCP](../articles/es/mcp-remote-management-tools.md) |

Estas comparaciones se centran en los flujos de trabajo. Las funciones varían según el producto, la edición y la configuración; las guías enlazadas explican cuándo puede convenir más una herramienta especializada.

## Empieza en el navegador

1. Visita [bastr.io](https://bastr.io/es/). Usa una conexión de invitado disponible para una sesión temporal o inicia sesión para guardar y organizar tu trabajo.
2. Elige un tipo de conexión e introduce el destino en **Quick Connect** o añádelo en **Hosts**. Introduce las contraseñas y las claves privadas únicamente en el formulario de conexión.
3. Selecciona un proxy o un host de salto SSH si el destino necesita una ruta de red específica.
4. Abre la sesión. Usa **Files**, el panel de bases de datos o **Docker** para la siguiente tarea y organiza las sesiones relacionadas con los controles de distribución.
5. Para trabajar en equipo, selecciona el espacio adecuado y comparte los recursos que necesitan sus miembros. Activa la autenticación de dos factores y guarda el material de recuperación antes de depender de la cuenta para el acceso diario.

El acceso de invitado tiene su propia disponibilidad y límites de uso. Los hosts guardados, las funciones de equipo y algunas herramientas requieren iniciar sesión o una cuenta con acceso a esas funciones.

## Gestión de Docker por SSH

Abre **Docker** en el espacio de trabajo y selecciona un host SSH al que tengas acceso. La vista de Docker reúne contenedores, Compose, imágenes, volúmenes, redes y el progreso de las tareas. Puedes consultar el estado de los contenedores y su uso de recursos, realizar las acciones de ciclo de vida compatibles e iniciar un despliegue desde las plantillas de aplicaciones disponibles, una imagen personalizada o una configuración de Compose compatible.

Si Docker no está instalado, la interfaz puede guiarte durante la instalación en los hosts Linux compatibles, después de que revises y confirmes la acción propuesta. La disponibilidad depende del host, tus permisos y las funciones a las que tengas acceso en ese momento. Consulta la [guía comparativa de Docker](../articles/es/docker-management-tools-by-scenario.md) para seguir un proceso práctico de evaluación.

## Conecta clientes de IA mediante MCP

Bastrio admite conexiones mediante Model Context Protocol (MCP) desde clientes como Claude Code, Codex, Cursor y VS Code. MCP complementa al asistente de IA integrado: permite que el cliente que elijas trabaje con hosts, archivos, bases de datos y rutas de red autorizados.

1. Abre **Tools → MCP API Keys** en el espacio de trabajo.
2. Crea una clave con los permisos y el plazo de validez que necesita tu cliente.
3. Selecciona el cliente y sigue las instrucciones de conexión que aparecen en esa página.
4. Conserva la clave en la configuración de secretos o de entorno que admita el cliente. Revisa las solicitudes de aprobación en el navegador y revoca el acceso cuando ya no sea necesario.

Usa el endpoint que aparece en tu cuenta. Las herramientas disponibles dependen de los permisos concedidos; el cliente debe descubrirlas a través del servicio MCP. Lee la [guía de MCP](../articles/es/mcp-remote-management-tools.md) para ver ejemplos de cómo combinarlo con el trabajo en SSH, bases de datos y Docker.

## Seis guías prácticas en diez idiomas

La [biblioteca de guías](../articles/README.md) contiene las seis comparativas publicadas en inglés, chino simplificado, chino tradicional, español, alemán, francés, japonés, coreano, malayo y ruso. Cada versión conserva el texto existente de los artículos, las ilustraciones, las preguntas frecuentes y un enlace a su página original de Bastr.io.

[English guides](../articles/en/README.md) · [简体中文指南](../articles/zh/README.md) · [繁體中文指南](../articles/zh-TW/README.md) · [日本語](../articles/ja/README.md) · [한국어](../articles/ko/README.md) · [Español](../articles/es/README.md) · [Deutsch](../articles/de/README.md) · [Français](../articles/fr/README.md) · [Bahasa Melayu](../articles/ms/README.md) · [Русский](../articles/ru/README.md)

## Preguntas frecuentes

### ¿Qué es Bastrio?

Bastrio es un espacio de trabajo en el navegador que combina WebSSH, transferencia de archivos, RDP/VNC, bases de datos, gestión de Docker, recursos compartidos y asistencia con IA. Está pensado para desarrolladores y equipos de operaciones que trabajan con varios sistemas remotos.

### ¿Puede Bastrio sustituir a Termius, FinalShell o MobaXterm?

Bastrio ofrece un flujo de trabajo en el navegador para tareas habituales de SSH y gestión de archivos. Antes de cambiar de herramienta, evalúa las funciones de escritorio de las que dependes, como la integración con el shell local, las macros o X11. La [comparativa de SSH](../articles/es/ssh-tools-browser-workspace.md) te ayuda a elegir según el escenario.

### ¿Es Bastrio una alternativa en el navegador a Navicat o DBeaver?

Puede cubrir flujos de trabajo habituales con bases de datos remotas PostgreSQL, MySQL/MariaDB, SQL Server, Redis y MongoDB. Las operaciones disponibles varían según el motor y los permisos. El modelado avanzado, la sincronización y los procesos de desarrollo especializados deben evaluarse según tus requisitos.

### ¿Es Bastrio una alternativa a Portainer?

Para quienes quieren gestionar hosts Docker y Compose junto a SSH, archivos y bases de datos, Bastrio ofrece un flujo de trabajo en el navegador a través de una conexión SSH existente. Contrasta la [guía de Docker](../articles/es/docker-management-tools-by-scenario.md) con tu entorno y tus necesidades de despliegue.

### ¿Necesito instalar un cliente de escritorio?

Puedes usar el espacio de trabajo desde un navegador compatible. El destino sigue necesitando un servicio accesible de SSH, transferencia de archivos, escritorio remoto o bases de datos, además de credenciales de acceso válidas.

### ¿Cómo se protegen las credenciales de conexión y las notas sensibles?

Las credenciales de conexión guardadas se cifran en reposo con AES-256-GCM y Bastr.io usa HTTPS para el acceso desde el navegador. Los runbooks sensibles permiten guardar el contenido cifrado con una contraseña de documento independiente. La autenticación de dos factores, el material de recuperación y los permisos de los recursos aportan controles adicionales.

### ¿Puedo empezar sin una cuenta?

Usa una conexión de invitado cuando la página de inicio la ofrezca. El acceso de invitado, los protocolos y los tiempos permitidos pueden cambiar; inicia sesión para usar conexiones guardadas y las herramientas disponibles para tu cuenta.

## Contacto e información del proyecto

Sitio web: [bastr.io](https://bastr.io/es/) · Soporte: [sup@bastr.io](mailto:sup@bastr.io) · [Informar de un problema](https://github.com/cihalqe/bastrio/issues)

Este repositorio contiene la documentación pública del producto Bastrio y sus guías. Las sugerencias y correcciones son bienvenidas. Comparte únicamente ejemplos sin datos sensibles en las incidencias y solicitudes de cambios.

Licencia: [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).
