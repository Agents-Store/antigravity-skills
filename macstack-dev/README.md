# macstack-dev (Antigravity plugin)

MACSTACK dev plugin for Agents Store. Creates and maintains the macstack/ folder of a Claude project: macstack.json — the standardized business + technical stack specification — plus the working documents around it: user cases per role, test cases derived from their acceptance bullets, milestones and tasks reconciled with the team's own task tracker, a typed development journal and its client-facing changelog, business logic in plain words, the decision log with cost-if-wrong, open questions split into what the client owes and what the team deferred, and an immutable inbox for client material. Init in existing projects, generate from scratch (result-first), discover context plugins and prototypes, scaffold project files in the prototype → stack plugins → dev plugins order, merge incoming client edits through a gated delta/rulings loop, report where the project stands and what to run next, wire Infisical env, install best-practice rules and commands.

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
