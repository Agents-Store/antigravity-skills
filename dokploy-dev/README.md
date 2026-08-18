# dokploy-dev (Antigravity plugin)

Dokploy self-hosted PaaS development plugin (aligned with Dokploy v0.29.14). Deploy applications, provision 6 database types (Postgres, MySQL, MariaDB, MongoDB, Redis, LibSQL), manage domains and Docker Compose stacks, AND debug failed deployments end-to-end — reads runtime logs of every container (including each container in a Docker Compose stack) over the API/MCP with tail/since/search, plus AI-powered log analysis (ai-analyzeLogs), Docker container introspection, Traefik diagnosis, and a guided recovery chain. Complete MCP/REST coverage: all 546 v0.29.14 operations across 50 categories indexed with params — covers forward-auth SSO domain protection, SCIM provisioning, build concurrency, and the rewritten @dokploy/cli (546 auto-generated commands incl. read-logs). Uses the official @dokploy/mcp server plus debugging-focused slash commands including /compose-logs.

## Install

Workspace-scoped:
```bash
agy plugin install ./dokploy-dev
```
Copies this directory to `.agents/plugins/dokploy-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./dokploy-dev
```
Copies this directory to `~/.gemini/config/plugins/dokploy-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `DOKPLOY_API_KEY`
- `DOKPLOY_URL`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/dokploy-dev
