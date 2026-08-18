# stack-directus-nextjs-trigger-dev (Antigravity plugin)

Directus + Next.js + Trigger.dev stack dev plugin. Adds self-hosted Trigger.dev as a workflow engine for AI agents, durable async logic, and scheduled jobs on top of the Directus + Next.js App Router stack.

## Install

Workspace-scoped:
```bash
agy plugin install ./stack-directus-nextjs-trigger-dev
```
Copies this directory to `.agents/plugins/stack-directus-nextjs-trigger-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./stack-directus-nextjs-trigger-dev
```
Copies this directory to `~/.gemini/config/plugins/stack-directus-nextjs-trigger-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `DIRECTUS_ADMIN_TOKEN`
- `NEXT_PUBLIC_DIRECTUS_URL`
- `TRIGGER_API_URL`
- `TRIGGER_SECRET_KEY`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/stack-directus-nextjs-trigger-dev
