# web-search-dev (Antigravity plugin)

Developer reference for web search, scraping and documentation lookup — Firecrawl, Exa, Jina, Perplexity, Context7 MCP tools and REST/SDK/CLI — plus Pexels and Unsplash REST media search.

## Install

Workspace-scoped:
```bash
agy plugin install ./web-search-dev
```
Copies this directory to `.agents/plugins/web-search-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./web-search-dev
```
Copies this directory to `~/.gemini/config/plugins/web-search-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `CONTEXT7_API_KEY`
- `EXA_API_KEY`
- `FIRECRAWL_API_TOKEN`
- `JINA_API_KEY`
- `PERPLEXITY_API_KEY`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/web-search-dev
