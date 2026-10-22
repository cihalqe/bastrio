# Bastrio MCP plugin

[Bastrio](https://bastr.io/mcp.html) connects your AI client to remote servers,
SSH terminals, files, databases and proxies with scoped access and user approvals.
It is a hosted service: you need a Bastrio account, an authorized workspace and
permission to access the resources you want to use. Pricing and quotas follow
your account plan.

## Install from a plugin directory

This repository contains an [Agent Plugins 1.0.0](https://open-plugins.com/specification)
package at its root. `plugin.json` identifies the plugin and `mcp.json` registers
the Streamable HTTP server at `https://bastr.io/api/mcp`. No local server process
or package installation is needed.

Install or enable the Bastrio plugin in a compatible client. Connect to its MCP
server and complete the browser authorization when your client prompts you.
An initial HTTP 401 is expected before authorization. Authorization and stored
credentials are managed by your client.

## Connect directly in Cursor

Clients that do not load the portable plugin format can connect directly.
Add this to your Cursor MCP configuration using its settings UI or
`.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "bastrio": {
      "url": "https://bastr.io/api/mcp"
    }
  }
}
```

Enable Bastrio and use the client's browser authentication flow. If your client
requires an API key instead, create a scoped key in
[Bastrio MCP API Keys](https://bastr.io/workspace/integrations/mcp/api-keys)
and configure `Authorization: Bearer <your key>` using the client's credential
settings. Keep credentials in your private client configuration.

The portable `mcp.json` intentionally contains only the public endpoint. Agent
Plugins 1.0.0 does not define portable secret inputs or environment expansion in
HTTP headers; authorization belongs to the client.

## Use the tools

Start with `identity.get` and discover the available tools with `tools/list`.
Tool availability follows your granted permissions. When a result requires
approval, follow its browser approval instructions before continuing.

Examples:

- List the servers available in my authorized workspace.
- Read a configuration file on a server I can access.
- Run a read-only query against an authorized database.
- Show the approvals waiting for my review.

## Submit this repository to Cursor Directory

On the directory's **Submit a Plugin** page, select **Auto (GitHub)** and scan
`https://github.com/cihalqe/bastrio`. Use the repository root. The scanner should
discover `mcp.json` as the MCP component and use `plugin.json` for plugin metadata.

The plugin configuration must be present on the branch scanned by the directory
(normally `main`) before scanning again. A local file or an unmerged branch is
not visible to that scanner. Directory review and acceptance are separate from
the package format validation.
