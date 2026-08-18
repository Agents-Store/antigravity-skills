# multi-bank (Antigravity plugin)

Multi-Bank Account Manager with broadcast architecture pattern. Aggregates financial data from Monobank and PrivatBank via MCP tools, broadcasts balance updates and budget alerts to subscribed components, categorizes transactions, and exports financial reports in CSV/PDF.

## Install

Workspace-scoped:
```bash
agy plugin install ./multi-bank
```
Copies this directory to `.agents/plugins/multi-bank/` in the current workspace.

Global:
```bash
agy plugin install --global ./multi-bank
```
Copies this directory to `~/.gemini/config/plugins/multi-bank/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `MONOBANK_MCP_URL`
- `PRIVATBANK_MCP_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/multi-bank
