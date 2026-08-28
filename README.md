# Basedash agent plugin

Basedash MCP packaged for agent clients. One hosted server, OAuth, no API keys.

- **MCP:** `https://charts.basedash.com/api/public/mcp`
- **Data tools:** `ask_question`, `get_data_sources`
- **Dashboard and chart tools:** `list_dashboards`, `get_dashboard`, `create_dashboard`, `edit_dashboard`, `list_charts`, `get_chart`, `create_chart`, `edit_chart`
- **Logo:** `logo.svg`

The MCP server uses the same workspace permissions as the Basedash app. Dashboard and chart reads are access-control aware. OAuth includes `mcp:dashboards:read` and `mcp:dashboards:write`; existing connections were backfilled and do not need to re-authenticate.

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
- `inspect-dashboards-and-charts` — list and inspect accessible dashboards and charts
- `manage-dashboards-and-charts` — create and edit dashboards and charts with natural-language instructions

## Links

- [Basedash](https://www.basedash.com)
- [MCP server docs](https://www.basedash.com/docs/features/mcp-server)
- [This repo](https://github.com/Basedash/agent-plugin)
