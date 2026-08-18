# vercel-dev (Antigravity plugin)

Vercel ecosystem plugin. Deployment, AI SDK, Edge Functions, storage, routing, performance optimization. Includes CLI deploy troubleshooting for non-Git projects, Hobby plan fixes, standalone output handling. Based on official vercel-plugin v0.25.0 by Vercel Labs.

## Install

Workspace-scoped:
```bash
agy plugin install ./vercel-dev
```
Copies this directory to `.agents/plugins/vercel-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./vercel-dev
```
Copies this directory to `~/.gemini/config/plugins/vercel-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:


## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/vercel-dev
