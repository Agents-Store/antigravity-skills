# nocobase (Antigravity plugin)

NocoBase platform development plugin. Expert guidance on collections, fields, relations, workflows, UI blocks, plugin development, MCP-powered page management, data operations, and collection inspection for NocoBase applications.

## Install

Workspace-scoped:
```bash
agy plugin install ./nocobase
```
Copies this directory to `.agents/plugins/nocobase/` in the current workspace.

Global:
```bash
agy plugin install --global ./nocobase
```
Copies this directory to `~/.gemini/config/plugins/nocobase/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `NOCOBASE_EMAIL`
- `NOCOBASE_PASSWORD`
- `NOCOBASE_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/nocobase
