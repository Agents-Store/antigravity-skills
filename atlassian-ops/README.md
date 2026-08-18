# atlassian-ops (Antigravity plugin)

Atlassian Jira + Confluence Cloud ops plugin. Drive the full Jira Cloud REST API v3 and Confluence Cloud REST API v2 by curl — Jira: issues (create/edit/transition/assign, ADF bodies), JQL search, comments & worklogs, attachments & links, projects/versions/components, fields & screens, workflows/types/statuses, users & groups (accountId), permission/notification/security schemes, dashboards & filters, plans & teams; Confluence: pages & blog posts (versioned, storage/ADF bodies), spaces & permissions, comments & attachments, labels & content properties. Authenticates with Atlassian Cloud Basic auth (ATLASSIAN_EMAIL + ATLASSIAN_API_TOKEN) against ATLASSIAN_SITE_URL.

## Install

Workspace-scoped:
```bash
agy plugin install ./atlassian-ops
```
Copies this directory to `.agents/plugins/atlassian-ops/` in the current workspace.

Global:
```bash
agy plugin install --global ./atlassian-ops
```
Copies this directory to `~/.gemini/config/plugins/atlassian-ops/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/atlassian-ops
