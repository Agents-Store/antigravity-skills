# codemap-dev (Antigravity plugin)

Code understanding plugin for developers. Helps onboard to unfamiliar projects through beginner-friendly code review, step-by-step explanations, visual diagrams (architecture, ERD, flows) via drawio-mcp, and frontend testing via Playwright MCP.

## Install

Workspace-scoped:
```bash
agy plugin install ./codemap-dev
```
Copies this directory to `.agents/plugins/codemap-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./codemap-dev
```
Copies this directory to `~/.gemini/config/plugins/codemap-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:


## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/codemap-dev
