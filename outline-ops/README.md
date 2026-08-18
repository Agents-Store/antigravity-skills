# outline-ops (Antigravity plugin)

Outline knowledge-base ops plugin. Drive the full Outline REST API by curl — documents (create, search, move, archive, trash, import/export, AI answers, memberships), collections (CRUD, user/group permissions, export), comments, stars, views, shares & access requests, users & groups, attachments & file operations, revisions, templates, events (audit log), OAuth clients, and data attributes. Authenticates with a Bearer OUTLINE_API_KEY against OUTLINE_API_URL.

## Install

Workspace-scoped:
```bash
agy plugin install ./outline-ops
```
Copies this directory to `.agents/plugins/outline-ops/` in the current workspace.

Global:
```bash
agy plugin install --global ./outline-ops
```
Copies this directory to `~/.gemini/config/plugins/outline-ops/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/outline-ops
