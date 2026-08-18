# macstack-dev (Antigravity plugin)

MACSTACK dev plugin for Agents Store. Creates and maintains macstack.json — the standardized business + technical stack specification for Claude projects: init in existing projects, generate from scratch (result-first), discover context plugins and prototypes, scaffold project files in the prototype → stack plugins → dev plugins order, wire Infisical env, install best-practice rules and commands.

## Install

Workspace-scoped:
```bash
agy plugin install ./macstack-dev
```
Copies this directory to `.agents/plugins/macstack-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./macstack-dev
```
Copies this directory to `~/.gemini/config/plugins/macstack-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/macstack-dev
