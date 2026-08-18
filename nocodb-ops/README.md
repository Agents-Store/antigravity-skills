# nocodb-ops (Antigravity plugin)

NocoDB ops plugin for Agents Store. Record management, views, reports, filtering, search, and data import/export for business users via MCP tools and CLI.

## Install

Workspace-scoped:
```bash
agy plugin install ./nocodb-ops
```
Copies this directory to `.agents/plugins/nocodb-ops/` in the current workspace.

Global:
```bash
agy plugin install --global ./nocodb-ops
```
Copies this directory to `~/.gemini/config/plugins/nocodb-ops/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `NOCODB_MCP_TOKEN`
- `NOCODB_MCP_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/nocodb-ops
