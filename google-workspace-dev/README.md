# google-workspace-dev (Antigravity plugin)

Google Workspace plugin powered by the official googleworkspace/cli (gws) Agent Skills. ~95 skills for Gmail, Drive, Calendar, Sheets, Docs, Chat, Meet, Tasks, Slides, Forms, Classroom and Admin — plus role personas and ready-made recipes — all driving the gws CLI. Vendored from upstream and auto-synced weekly. Requires the gws CLI (npm i -g @googleworkspace/cli) and a one-time OAuth setup.

## Install

Workspace-scoped:
```bash
agy plugin install ./google-workspace-dev
```
Copies this directory to `.agents/plugins/google-workspace-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./google-workspace-dev
```
Copies this directory to `~/.gemini/config/plugins/google-workspace-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/google-workspace-dev
