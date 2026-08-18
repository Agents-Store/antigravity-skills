# deep-research (Antigravity plugin)

Deep Research plugin. Comprehensive web research using 4 providers (Exa, Firecrawl, Jina, Perplexity) with capability-based CONNECTORS pattern and automatic FALLBACK chains. Search, scrape, crawl, extract — each action tries multiple providers until one succeeds.

## Install

Workspace-scoped:
```bash
agy plugin install ./deep-research
```
Copies this directory to `.agents/plugins/deep-research/` in the current workspace.

Global:
```bash
agy plugin install --global ./deep-research
```
Copies this directory to `~/.gemini/config/plugins/deep-research/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:


## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/deep-research
