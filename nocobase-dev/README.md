# nocobase-dev (Antigravity plugin)

NocoBase v2 development plugin. Build, manage, and operate NocoBase through the `nb` CLI (primary) or REST API (fallback). Bundles 11 official upstream skills from nocobase/skills (auto-synced weekly via GitHub Action), 5 custom REST-API skills (overview, auth, cli-recipes, api-reference, examples), and the full OpenAPI 3.0.3 spec for NocoBase v2.1.0-beta.29 (272 endpoints across 19 tag groups). No MCP server. Env vars match upstream naming: NB_URL + NB_USER + NB_PASSWORD for sign-in flow, or NB_URL + NB_TOKEN for the long-lived API Key path.

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
