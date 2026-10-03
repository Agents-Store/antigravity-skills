# stack-directus-nextjs (Antigravity plugin)

Directus + Next.js architecture plugin. How Directus (content, files, access) and a Next.js App Router frontend fit together: who holds the token, how the cache is invalidated, how assets and types cross the boundary, who owns the session, and a production checklist. Tool knowledge comes from its dependencies.

## Install

Workspace-scoped:
```bash
agy plugin install ./stack-directus-nextjs
```
Copies this directory to `.agents/plugins/stack-directus-nextjs/` in the current workspace.

Global:
```bash
agy plugin install --global ./stack-directus-nextjs
```
Copies this directory to `~/.gemini/config/plugins/stack-directus-nextjs/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `DIRECTUS_ADMIN_TOKEN`
- `NEXT_PUBLIC_DIRECTUS_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/stack-directus-nextjs
