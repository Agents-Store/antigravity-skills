# dify-ops (Antigravity plugin)

Dify self-hosted update operations plugin. Pre-flight the target release and the bundled Weaviate migration path, back up volumes with the stack down, merge a release tag into the local dev branch, sync .env variables, and pull and restart containers for Dify Docker deployments.

## Install

Workspace-scoped:
```bash
agy plugin install ./dify-ops
```
Copies this directory to `.agents/plugins/dify-ops/` in the current workspace.

Global:
```bash
agy plugin install --global ./dify-ops
```
Copies this directory to `~/.gemini/config/plugins/dify-ops/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/dify-ops
