# nocobase-dev (Antigravity plugin)

NocoBase v2 development plugin. Build, manage, and operate NocoBase through the `nb` CLI 2.2 (primary) or REST API (fallback). Bundles 20 official upstream skills from nocobase/skills (auto-synced weekly via GitHub Action; UI authoring enters through nocobase-portal-manage), 5 custom skills (overview, auth, cli-recipes, api-reference, examples), and an OpenAPI 3.0.3 snapshot of NocoBase v2.1.0-beta.29 (272 endpoints; refresh from a 2.2.x stand pending). Targets the stable @nocobase/cli channel (Node.js 22+); NocoBase 2.1.0+ for agent connection. No MCP server shipped; NocoBase has its own at /api/mcp. Env vars match upstream naming: NB_URL + NB_USER + NB_PASSWORD for sign-in flow, or NB_URL + NB_TOKEN for the long-lived API Key path.

## Install

Workspace-scoped:
```bash
agy plugin install ./nocobase-dev
```
Copies this directory to `.agents/plugins/nocobase-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./nocobase-dev
```
Copies this directory to `~/.gemini/config/plugins/nocobase-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/nocobase-dev
