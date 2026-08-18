# mem0 (Antigravity plugin)

Mem0 memory management plugin. Store, search, update, and organize memories with semantic search, batch operations, file attachments, and change history tracking via MCP tools.

## Install

Workspace-scoped:
```bash
agy plugin install ./mem0
```
Copies this directory to `.agents/plugins/mem0/` in the current workspace.

Global:
```bash
agy plugin install --global ./mem0
```
Copies this directory to `~/.gemini/config/plugins/mem0/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:


## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/mem0
