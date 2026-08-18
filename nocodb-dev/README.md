# nocodb-dev (Antigravity plugin)

NocoDB schema development plugin. Full Meta API v3 coverage — tables, fields (30+ types), views, filters, sorts, hooks (HookV3), comments, scripts, dashboards & widgets, workflows, plus workspaces / members / teams / tokens. Bundles both Data API and Meta API OpenAPI specs.

## Install

Workspace-scoped:
```bash
agy plugin install ./nocodb-dev
```
Copies this directory to `.agents/plugins/nocodb-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./nocodb-dev
```
Copies this directory to `~/.gemini/config/plugins/nocodb-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `NOCODB_MCP_TOKEN`
- `NOCODB_MCP_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/nocodb-dev
