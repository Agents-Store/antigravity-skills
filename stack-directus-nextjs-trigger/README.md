# stack-directus-nextjs-trigger (Antigravity plugin)

Directus + Next.js + Trigger.dev architecture plugin. How Directus (content, files, access), a Next.js App Router frontend and self-hosted Trigger.dev (durable and scheduled work) fit together: who holds which token, how the cache is invalidated, how a Directus change reaches a task and the result reaches the page, who owns the session, and a production checklist. Tool knowledge comes from its dependencies.

## Install

Workspace-scoped:
```bash
agy plugin install ./stack-directus-nextjs-trigger
```
Copies this directory to `.agents/plugins/stack-directus-nextjs-trigger/` in the current workspace.

Global:
```bash
agy plugin install --global ./stack-directus-nextjs-trigger
```
Copies this directory to `~/.gemini/config/plugins/stack-directus-nextjs-trigger/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `DIRECTUS_ADMIN_TOKEN`
- `NEXT_PUBLIC_DIRECTUS_URL`
- `TRIGGER_ACCESS_TOKEN`
- `TRIGGER_API_URL`
- `TRIGGER_PROJECT_REF`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/stack-directus-nextjs-trigger
