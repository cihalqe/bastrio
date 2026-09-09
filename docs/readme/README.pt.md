<p align="center">
  <a href="https://bastr.io/en/"><img src="../images/readme/bastrio-wordmark.png" width="340" alt="Bastrio" /></a>
</p>

# Bastrio — WebSSH, desktops remotos, bancos de dados e Docker no navegador

[Bastrio (Bastr.io)](https://bastr.io/en/) é um espaço de trabalho no navegador para gerenciar servidores remotos. Abra um terminal SSH online, transfira arquivos por SFTP, acesse desktops RDP ou VNC, trabalhe com bancos de dados e gerencie hosts Docker no mesmo lugar. Conexões salvas, abas, painéis divididos, espaços compartilhados e assistência de IA mantêm as tarefas relacionadas juntas, com armazenamento criptografado de credenciais e proteção da conta.

[Abrir espaço de trabalho](https://bastr.io/workspace/) · [Biblioteca de guias](../articles/README.md) · [Site em inglês](https://bastr.io/en/)

[English](../../README.md) · [简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Español](README.es.md) · [Deutsch](README.de.md) · [Français](README.fr.md) · Português · [العربية](README.ar.md)

## Um espaço de trabalho que acompanha a tarefa

Conecte-se a um host, abra o terminal, examine um arquivo de configuração, consulte o banco de dados e verifique um contêiner sem recriar o contexto de conexão em vários aplicativos. A barra de hosts, as abas e os painéis divididos mantêm as ferramentas próximas do trabalho.

![Espaço de trabalho Bastrio com terminal SSH e gerenciador SFTP em painéis divididos](../images/readme/split-workspace.png)

| Área | O que você pode fazer na interface |
| --- | --- |
| Hosts e sessões | Salvar conexões, organizar pastas, filtrar tipos, reabrir sessões recentes e distribuir abas ou painéis. |
| WebSSH e comandos remotos | Usar autenticação por senha ou chave SSH, terminal no navegador, comandos rápidos, pesquisa e reconexão. WinRM e Telnet também estão disponíveis quando habilitados. |
| SFTP, FTP e FTPS | Navegar por diretórios, enviar e baixar arquivos, criar pastas, renomear e editar arquivos de texto compatíveis junto ao terminal. |
| RDP e VNC | Abrir desktops remotos no navegador com controles de sessão, área de transferência e atalhos. O destino precisa oferecer um serviço RDP ou VNC acessível. |
| Bancos de dados | Conectar PostgreSQL, MySQL/MariaDB, SQL Server, Redis e MongoDB e usar os recursos de navegação, consulta, edição e backup disponíveis para cada mecanismo. |
| Docker | Adicionar um host SSH existente, descobrir contêineres, consultar uso de recursos e trabalhar com contêineres, Compose, imagens, volumes e redes. Implantar com modelos de aplicativos, imagens personalizadas ou configurações Compose compatíveis. |
| Caminhos de rede | Escolher uma rota de proxy regional disponível, configurar seu próprio proxy ou usar um host de salto SSH. |
| Espaços compartilhados | Alternar entre espaços pessoais e de equipe, convidar membros e conceder acesso aos recursos necessários. |
| IA e MCP | Pedir ajuda junto ao terminal ou banco de dados ou conectar um cliente MCP aos recursos autorizados. |
| Documentos criptografados e armazenamento | Organizar documentos, criptografar notas sensíveis com senha independente e gerenciar arquivos no espaço disponível. |

Protocolos, ações do Docker, gravações em bancos de dados, uso de IA e armazenamento dependem da conta, das permissões do espaço e do serviço de destino. A interface mostra as opções disponíveis na sessão.

## Criptografia e controle de acesso

- **Credenciais criptografadas:** senhas de conexão e chaves privadas salvas são protegidas em repouso com AES-256-GCM.
- **Transporte protegido:** acesse Bastr.io por HTTPS e escolha protocolos remotos criptografados adequados ao destino, como SSH/SFTP ou FTPS.
- **Proteção da conta:** habilite a autenticação de dois fatores e guarde a chave de recuperação offline. O processo de recuperação ajuda a restaurar o acesso às credenciais criptografadas após redefinir a senha.
- **Documentos com senha própria:** selecione o modo criptografado, defina uma senha independente e confirme a criptografia e o salvamento no editor. Guarde essa senha com cuidado.
- **Acesso de IA controlado:** chaves de API MCP têm permissões selecionadas, validade e revogação. Revise solicitações de aprovação no navegador e gerencie as credenciais dos servidores pela interface do espaço de trabalho.

Essas proteções se somam às permissões e à segurança dos sistemas remotos. Mantenha credenciais reais e materiais de recuperação fora de documentos compartilhados, capturas de tela e conversas com IA.

## Alternativas a ferramentas SSH, de banco de dados e Docker

Ao procurar uma alternativa ao Termius, uma forma de trabalhar no navegador em vez de FinalShell ou Xshell, um cliente de banco de dados semelhante ao Navicat ou uma alternativa ao Portainer via SSH, comece pela tarefa. Bastrio reúne diferentes recursos remotos em um fluxo compartilhado no navegador.

| Ferramentas em comparação | Quando considerar Bastrio | Guia em inglês |
| --- | --- | --- |
| Termius, FinalShell, MobaXterm, Xshell, SecureCRT e PuTTY | SSH no navegador, hosts salvos, sessões divididas e arquivos próximos. Avalie requisitos de scripts de desktop e X11 separadamente. | [Ferramentas SSH](../articles/en/ssh-tools-browser-workspace.md) |
| WinSCP, FileZilla, Xftp e Cyberduck | Transferências SFTP ou FTP/FTPS e edição de texto junto à sessão remota. | [Fluxo FTP/SFTP](../articles/en/ftp-sftp-tools-browser-workflow.md) |
| Navicat, DBeaver, DataGrip, pgAdmin, Redis Insight e MongoDB Compass | Banco de dados no navegador ao lado dos hosts, conforme as necessidades de consulta, edição e backup de cada mecanismo. | [Bancos de dados remotos](../articles/en/remote-database-tools-comparison.md) |
| Apache Guacamole, TeamViewer, AnyDesk e ToDesk | Acesso pelo navegador a um destino RDP/VNC existente. Assistência remota e gateways de desktop têm requisitos de conexão distintos. | [Desktops remotos](../articles/en/browser-remote-desktop-tools.md) |
| Portainer, Dockge e Docker Desktop | Gerenciamento remoto de Docker e Compose por um host SSH existente. Desenvolvimento local e gestão de clusters exigem avaliação própria. | [Docker por cenário](../articles/en/docker-management-tools-by-scenario.md) |
| MCP junto a SSH, bancos de dados e Docker | Um cliente de IA acessando recursos autorizados, com permissões e controles de aprovação. | [Gerenciamento via MCP](../articles/en/mcp-remote-management-tools.md) |

A comparação trata de fluxos de trabalho. Os recursos variam por produto, edição e configuração; os guias também explicam quando uma ferramenta especializada pode ser mais adequada.

## Começar no navegador

1. Visite [bastr.io](https://bastr.io/en/). Use uma conexão de visitante disponível para uma sessão temporária ou entre na conta para salvar seu trabalho.
2. Escolha o protocolo em **Quick Connect** ou adicione um destino em **Hosts**. Digite senhas e chaves privadas apenas no formulário de conexão.
3. Selecione um proxy ou host de salto SSH quando precisar de um caminho de rede específico.
4. Abra a sessão e use **Files**, o painel de banco de dados ou **Docker** para continuar a tarefa. Organize sessões relacionadas com os controles de layout.
5. Para trabalhar em equipe, selecione o espaço correto e compartilhe os recursos necessários. Habilite dois fatores e guarde o material de recuperação.

Conexões de visitante têm disponibilidade e limites próprios. Hosts salvos, colaboração e determinadas ferramentas exigem login ou uma conta elegível.

## Gerenciar Docker por SSH

Abra **Docker** e selecione um host SSH ao qual você tenha acesso. A interface reúne contêineres, Compose, imagens, volumes, redes e progresso de tarefas. Consulte estado e consumo de recursos, execute ações de ciclo de vida compatíveis e inicie uma implantação com modelos de aplicativos, imagem personalizada ou configuração Compose compatível.

Se o Docker não estiver instalado, a interface pode orientar a instalação em hosts Linux compatíveis após sua revisão e confirmação. A disponibilidade depende do host, das permissões e do acesso atual à funcionalidade. Veja o [guia de Docker em inglês](../articles/en/docker-management-tools-by-scenario.md).

## Conectar clientes de IA por MCP

Bastrio oferece conexões Model Context Protocol (MCP) para clientes como Claude Code, Codex, Cursor e VS Code. Além do assistente de IA integrado, seu cliente pode trabalhar com hosts, arquivos, bancos de dados e caminhos de rede autorizados.

1. Abra **Tools → MCP API Keys**.
2. Crie uma chave com as permissões e a validade necessárias.
3. Selecione o cliente e siga as instruções de conexão da página.
4. Guarde a chave na configuração de segredos ou variáveis de ambiente suportada pelo cliente, revise as aprovações no navegador e revogue o acesso quando deixar de ser necessário.

Use o endereço exibido na sua conta. O cliente deve descobrir as ferramentas disponíveis no serviço MCP de acordo com as permissões concedidas. Leia o [guia MCP em inglês](../articles/en/mcp-remote-management-tools.md).

## Seis guias em dez idiomas

A [biblioteca de guias](../articles/README.md) reúne seis comparações publicadas em inglês, chinês simplificado, chinês tradicional, espanhol, alemão, francês, japonês, coreano, malaio e russo. As cópias preservam as traduções existentes, imagens, perguntas frequentes e links para os originais. Os links de comparação desta página levam às versões em inglês; não há tradução desses artigos para português nesta coleção.

[English](../articles/en/README.md) · [简体中文](../articles/zh/README.md) · [繁體中文](../articles/zh-TW/README.md) · [日本語](../articles/ja/README.md) · [한국어](../articles/ko/README.md) · [Español](../articles/es/README.md) · [Deutsch](../articles/de/README.md) · [Français](../articles/fr/README.md) · [Bahasa Melayu](../articles/ms/README.md) · [Русский](../articles/ru/README.md)

## Perguntas frequentes

### O que é Bastrio?

É um espaço de trabalho no navegador que reúne WebSSH, transferência de arquivos, RDP/VNC, bancos de dados, Docker, recursos compartilhados e assistência de IA para desenvolvedores e operadores.

### Bastrio pode substituir Termius, FinalShell ou MobaXterm?

Oferece um fluxo no navegador para tarefas comuns de SSH e arquivos. Confira dependências de integração com o shell local, macros ou X11 antes de mudar. O [guia SSH em inglês](../articles/en/ssh-tools-browser-workspace.md) ajuda a escolher por cenário.

### É uma alternativa no navegador ao Navicat ou DBeaver?

Pode atender tarefas comuns com PostgreSQL, MySQL/MariaDB, SQL Server, Redis e MongoDB. Operações variam conforme o mecanismo e as permissões; avalie modelagem avançada, sincronização e desenvolvimento especializado conforme seus requisitos.

### É uma alternativa ao Portainer?

Pode ser avaliado para gerenciamento de hosts Docker e Compose junto a SSH, arquivos e bancos de dados, usando uma conexão SSH existente. Compare o [guia de Docker em inglês](../articles/en/docker-management-tools-by-scenario.md) com as necessidades do ambiente.

### Preciso instalar um cliente de desktop?

O espaço de trabalho funciona em um navegador compatível. O destino precisa oferecer um serviço remoto acessível e credenciais válidas.

### Como são protegidas as credenciais e notas sensíveis?

Credenciais salvas usam AES-256-GCM em repouso e o acesso ao site usa HTTPS. Documentos sensíveis permitem salvamento criptografado com senha própria. Dois fatores, recuperação e permissões complementam a proteção.

### Posso usar sem conta?

Use o acesso de visitante quando estiver disponível na página inicial. Protocolos e limites de tempo podem variar. Entre na conta para salvar conexões e usar as ferramentas disponíveis para seu perfil.

## Contato e informações do projeto

Site: [bastr.io](https://bastr.io/en/) · Suporte: [sup@bastr.io](mailto:sup@bastr.io) · [Relatar um problema](https://github.com/cihalqe/bastrio/issues)

Este repositório contém a documentação pública e os guias do Bastrio. Sugestões e correções são bem-vindas. Use exemplos sem informações sensíveis em issues e pull requests.

Licença: [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).
