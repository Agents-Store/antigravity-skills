# session-doctor-dev (Antigravity plugin)

Read-only audit of a Claude Code session: where it runs, what context it loaded, which model and effort it used, the skills it invoked, every HTTP request with its status code, and the status of each API token seen in the session — with concrete fixes.

## Install

Workspace-scoped:
```bash
agy plugin install ./session-doctor-dev
```
Copies this directory to `.agents/plugins/session-doctor-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./session-doctor-dev
```
Copies this directory to `~/.gemini/config/plugins/session-doctor-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/session-doctor-dev
