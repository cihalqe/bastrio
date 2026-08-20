<p align="center"><a href="https://bastr.io/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a></p>

<p align="center">Un espacio de trabajo en el navegador para acceso remoto seguro, operaciones de infraestructura y colaboración.</p>

<p align="center"><a href="https://bastr.io/"><strong>bastr.io</strong></a> &nbsp;|&nbsp; <a href="https://www.gnu.org/licenses/gpl-3.0.html"><img src="https://img.shields.io/badge/license-GPL--3.0--only-2b82f0.svg" alt="GPL-3.0-only" /></a></p>

<p align="center"><a href="../../README.md">English</a> | <a href="README.zh-CN.md">简体中文</a> | <a href="README.zh-TW.md">繁體中文</a> | <a href="README.ja.md">日本語</a> | <a href="README.ko.md">한국어</a> | <strong>Español</strong> | <a href="README.de.md">Deutsch</a> | <a href="README.fr.md">Français</a> | <a href="README.pt.md">Português</a> | <a href="README.ar.md">العربية</a></p>

## Un espacio de trabajo para infraestructura remota

[Bastrio](https://bastr.io/) reúne **SSH online**, SFTP, FTP/FTPS, RDP, VNC y conexiones de bases de datos en un único espacio de trabajo del navegador. Úsalo como terminal web SSH, gestor de archivos online, cliente de base de datos en el navegador o espacio compartido para gestionar servidores remotos.

![Bastrio SSH online y acceso remoto desde el navegador](../images/readme/ssh-online-guest.png)

## Capacidades principales

- **Conecta desde el navegador:** terminal SSH online, archivos por SFTP/FTP/FTPS y escritorios remotos RDP y VNC.
- **Herramientas de base de datos unificadas:** PostgreSQL, MySQL/MariaDB, SQL Server, Redis y MongoDB en el mismo espacio de trabajo.
- **Organiza conexiones reales:** conexiones guardadas, carpetas, filtros por tipo, recientes, varias sesiones y paneles divididos.
- **Elige la ruta de red:** proxy IP por región, proxy personalizado o un host de salto SSH para infraestructura no expuesta directamente.
- **Asistencia con IA:** el asistente de IA ayuda a interpretar salidas, preparar comandos y acompañar el trabajo de terminal y base de datos.
- **Espacios colaborativos:** los espacios de trabajo y recursos compartidos conservan el contexto de conexión del equipo.
- **Documentos operativos cifrados:** redacta, cifra y guarda notas, borradores y texto sensible dentro del espacio de trabajo.

<p align="center"><img src="../images/readme/ssh-online-terminal.png" width="49%" alt="Terminal SSH online de Bastrio" /> <img src="../images/readme/connection-types.png" width="49%" alt="Tipos de conexión de Bastrio" /></p>

<p align="center"><img src="../images/readme/remote-workspace.png" width="49%" alt="Espacio remoto de Bastrio" /> <img src="../images/readme/sftp-file-browser.png" width="49%" alt="Explorador de archivos SFTP de Bastrio" /></p>

<p align="center"><img src="../images/readme/proxy-region-picker.png" width="49%" alt="Selector de región proxy de Bastrio" /> <img src="../images/readme/split-workspace.png" width="49%" alt="Espacio dividido de Bastrio" /></p>

<p align="center"><img src="../images/readme/postgresql-workspace.png" width="49%" alt="Espacio PostgreSQL de Bastrio" /> <img src="../images/readme/encrypted-operations-documents.png" width="49%" alt="Documentos operativos cifrados de Bastrio" /></p>

<p align="center"><img src="../images/readme/recovery-key.png" width="49%" alt="Clave de recuperación de Bastrio" /></p>

## Rutas de red bajo tu control

Bastrio permite usar la ruta adecuada para cada acceso remoto desde el navegador: selecciona un **proxy IP** si necesitas una región de salida, configura un proxy personalizado si quieres controlar el recorrido o usa un **host de salto SSH** para llegar a infraestructura privada. Estas opciones están junto a la conexión, no en otra herramienta.

## Trabajo remoto enfocado y colaborativo

Bastrio es un espacio remoto para desarrolladores, operadores y equipos que alternan entre servidores, archivos, escritorios y bases de datos. Los espacios de trabajo y recursos compartidos mantienen el contexto; las sesiones múltiples y los paneles divididos mantienen visible el trabajo relacionado; el asistente de IA permanece cerca de la tarea.

## Privacidad por diseño

Las credenciales y el contenido privado del espacio de trabajo se cifran en tránsito y en reposo. Bastrio descifra las credenciales solo temporalmente en la memoria volátil del servidor cuando una operación autorizada las requiere; el texto plano nunca se escribe en disco ni en registros. Todo acceso visible para el usuario requiere una sesión autenticada válida. Cuando una sesión caduca o se revoca, ya no es posible acceder a la bóveda cifrada ni descifrarla. La clave de recuperación se muestra una sola vez; es necesaria para restaurar credenciales cifradas después de restablecer la contraseña. Sin ella, la bóveda cifrada no se puede recuperar ni exportar de forma legible.

## Marketplace, previsto

Bastrio está preparando un Marketplace para servidores administrados y servicios de proxy IP. Son ofertas previstas para una versión futura, no servicios disponibles actualmente.

## Primeros pasos

1. Visita [bastr.io](https://bastr.io/) para abrir el espacio remoto Bastrio.
2. Elige SSH, transferencia de archivos, escritorio remoto o una conexión de base de datos.
3. Selecciona una ruta de red cuando sea necesario y guarda la conexión para organizar el trabajo posterior.

## Preguntas frecuentes

### ¿Es Bastrio una terminal web SSH?

Sí. Bastrio ofrece SSH online en el navegador junto con transferencia de archivos, escritorio remoto, bases de datos, proxy y herramientas de espacio de trabajo.

### ¿Puedo usar proxy IP, proxy personalizado y host de salto SSH?

Sí. Bastrio admite selección regional de proxy IP, configuración de proxy personalizado y hosts de salto SSH.

### ¿Puede el equipo colaborar en el mismo entorno?

Sí. Los espacios de trabajo y recursos compartidos están diseñados para mantener el trabajo de infraestructura remota organizado y colaborativo.

## Contribuciones

Se agradecen contribuciones e informes de problemas. Mantén las propuestas centradas en el comportamiento visible para el usuario y no incluyas credenciales ni datos de conexión privados en issues o pull requests.

## Licencia

Bastrio se publica bajo la [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).
