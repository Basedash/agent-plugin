# Basedash agent plugin

Basedash MCP packaged for agent clients. One hosted server, OAuth, no API keys.

- **MCP:** `https://charts.basedash.com/api/public/mcp`
- **Tools:** `ask_question`, `get_data_sources`
- **Logo:** `logo.svg`

Workspace access controls still apply after you sign in.

## Cursor

Install from the [Cursor Marketplace](https://cursor.com/marketplace) (listing is under review).

1. Open Cursor settings
2. Go to **Plugins**
3. Browse Marketplace and search for **Basedash**
4. Install, then complete the Basedash OAuth login

Repo layout for Cursor: `.cursor-plugin/plugin.json` and `mcp.json`.

## Claude

This repo is also a [Claude plugin](https://claude.com/docs/plugins/submit) (Cowork and Claude Code).

Until it is in the community directory:

```bash
claude --plugin-dir .
```

Or submit the public repo at [platform.claude.com/plugins/submit](https://platform.claude.com/plugins/submit).

Repo layout for Claude: `.claude-plugin/plugin.json` and `.mcp.json`.

## Skills

- `discover-company-data` — list connected sources via `get_data_sources`
- `analyze-company-data` — ask the AI data analyst via `ask_question` (pass `chat_id` to continue)

## Links

- [Basedash](https://www.basedash.com)
- [MCP server docs](https://www.basedash.com/docs/features/mcp-server)
- [This repo](https://github.com/Basedash/agent-plugin)
