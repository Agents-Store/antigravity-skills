# dataforseo-dev (Antigravity plugin)

DataForSEO data for SEO work — keywords, SERP, backlinks, on-page, AI visibility — through the v3 MCP server. Not a general web-search tool.

## Install

Workspace-scoped:
```bash
agy plugin install ./dataforseo-dev
```
Copies this directory to `.agents/plugins/dataforseo-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./dataforseo-dev
```
Copies this directory to `~/.gemini/config/plugins/dataforseo-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `DATAFORSEO_PASSWORD`
- `DATAFORSEO_USERNAME`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/dataforseo-dev
