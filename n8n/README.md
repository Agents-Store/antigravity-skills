# n8n (Antigravity plugin)

n8n workflow automation plugin. Manage workflows, execute automations, configure nodes, handle credentials, monitor executions, expression syntax, node configuration patterns, and code node best practices via MCP tools.

## Install

Workspace-scoped:
```bash
agy plugin install ./n8n
```
Copies this directory to `.agents/plugins/n8n/` in the current workspace.

Global:
```bash
agy plugin install --global ./n8n
```
Copies this directory to `~/.gemini/config/plugins/n8n/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `N8N_MCP_TOKEN`
- `N8N_MCP_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/n8n
