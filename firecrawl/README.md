# firecrawl (Antigravity plugin)

Firecrawl web scraping and search plugin. Scrape URLs, crawl sites, search the web, map site structures, extract structured data, batch scraping, autonomous research agents, and cloud browser sessions via MCP tools.

## Install

Workspace-scoped:
```bash
agy plugin install ./firecrawl
```
Copies this directory to `.agents/plugins/firecrawl/` in the current workspace.

Global:
```bash
agy plugin install --global ./firecrawl
```
Copies this directory to `~/.gemini/config/plugins/firecrawl/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `FIRECRAWL_MCP_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/firecrawl
