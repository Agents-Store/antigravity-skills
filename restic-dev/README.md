# restic-dev (Antigravity plugin)

restic backup plugin for Agents Store. Set up encrypted daily backups on any Linux server to S3-compatible storage (Cloudflare R2): server recon + restic install, auto-discovery of all Docker volumes/mounts and databases, R2 repository init, a partial-failure-tolerant backup script with logical DB dumps and retention, timezone-aware systemd/cron scheduling, verification, monitoring/dead-man's-switch, and disaster recovery. File-based knowledge, no MCP, no stored credentials.

## Install

Workspace-scoped:
```bash
agy plugin install ./restic-dev
```
Copies this directory to `.agents/plugins/restic-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./restic-dev
```
Copies this directory to `~/.gemini/config/plugins/restic-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/restic-dev
