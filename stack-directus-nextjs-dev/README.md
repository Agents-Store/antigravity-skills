# stack-directus-nextjs-dev (Antigravity plugin)

Directus + Next.js stack dev plugin. Integrates Directus headless CMS with Next.js App Router for content-driven applications.

## Install

Workspace-scoped:
```bash
agy plugin install ./stack-directus-nextjs-dev
```
Copies this directory to `.agents/plugins/stack-directus-nextjs-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./stack-directus-nextjs-dev
```
Copies this directory to `~/.gemini/config/plugins/stack-directus-nextjs-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `DIRECTUS_ADMIN_TOKEN`
- `NEXT_PUBLIC_DIRECTUS_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/stack-directus-nextjs-dev
