# chatwoot-dev (Antigravity plugin)

Chatwoot dev plugin for Agents Store. Full REST API coverage (Application, Platform, and Public/Client APIs) with bundled OpenAPI specs, official chatwoot CLI recipes, webhook & agent-bot automation, and troubleshooting for developers building on Chatwoot. Authenticates with the api_access_token header via CHATWOOT_API_KEY against CHATWOOT_BASE_URL.

## Install

Workspace-scoped:
```bash
agy plugin install ./chatwoot-dev
```
Copies this directory to `.agents/plugins/chatwoot-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./chatwoot-dev
```
Copies this directory to `~/.gemini/config/plugins/chatwoot-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/chatwoot-dev
