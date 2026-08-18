# openclaw-configurator (Antigravity plugin)

OpenClaw instance configurator and operations plugin. Scan, analyze, and optimize all workspace files (AGENTS.md, SOUL.md, USER.md, IDENTITY.md, TOOLS.md, HEARTBEAT.md, MEMORY.md, BOOT.md, BOOTSTRAP.md) plus openclaw.json. Update instances from official GitHub releases and reconcile config against new releases (recommend new features, migrate legacy settings, run openclaw doctor). Set up model-provider authentication with an OAuth/CLI-backend-first, cost-saving bias (Claude CLI, Codex OAuth). Migrate .env secrets into self-hosted Infisical. Guided interviews, session log analysis, standing orders design, security audit, config validation, permission fix hooks, centralized doc research, and 6 industry-specific workspace templates.

## Install

Workspace-scoped:
```bash
agy plugin install ./openclaw-configurator
```
Copies this directory to `.agents/plugins/openclaw-configurator/` in the current workspace.

Global:
```bash
agy plugin install --global ./openclaw-configurator
```
Copies this directory to `~/.gemini/config/plugins/openclaw-configurator/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/openclaw-configurator
