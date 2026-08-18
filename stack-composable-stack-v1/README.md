# stack-composable-stack-v1 (Antigravity plugin)

Composable Stack v1 dev plugin. Integrates PostgreSQL (direct MCP + PostgREST API), NocoDB, n8n, Trigger.dev, and NocoBase (prod + dev sandbox via nc-mcp) for building data-driven applications with low-code interfaces.

## Install

Workspace-scoped:
```bash
agy plugin install ./stack-composable-stack-v1
```
Copies this directory to `.agents/plugins/stack-composable-stack-v1/` in the current workspace.

Global:
```bash
agy plugin install --global ./stack-composable-stack-v1
```
Copies this directory to `~/.gemini/config/plugins/stack-composable-stack-v1/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `N8N_API_KEY`
- `N8N_API_URL`
- `N8N_MCP_TOKEN`
- `N8N_NATIVE_MCP_URL`
- `NOCOBASE_DEV_API_KEY`
- `NOCOBASE_DEV_URL`
- `NOCODB_MCP_URL`
- `NOCODB_TOKEN`
- `POSTGRESQL_MCP_TOKEN`
- `POSTGRESQL_MCP_URL`
- `TRIGGER_API_URL`
- `TRIGGER_SECRET_KEY`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/stack-composable-stack-v1
