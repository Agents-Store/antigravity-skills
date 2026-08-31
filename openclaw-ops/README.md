# openclaw-ops (Antigravity plugin)

Operations plugin for a fleet of self-hosted OpenClaw gateway instances running as Docker Compose projects on one host. Discovers every instance from the live Docker state (never from hard-coded paths), classifies it ok/degraded/down/alien, and runs day-two maintenance: health and liveness reporting, provider-auth triage (expired, emptied and shadowed OAuth profiles, shared-credential token sink), config surgery with snapshot and executable rollback, memory/embedding repair and reindexing, shared skills and plugins consolidation, Infisical secret-delivery audit by key name only, security audit, version-drift and channel-aware upgrades, and reference-instance cloning. Mutations are dry-run by default behind an eight-block plan, need --yes, and need a typed confirmation when irreversible. Secrets are reported as fingerprints, presence and expiry — never as values. File-based knowledge: no MCP server, no required environment variables, no stored credentials; the single optional variable OPENCLAW_OPS_CONFIG is an escape hatch for the fleet-config path, and deployment specifics live in that operator-owned config outside the repository.

## Install

Workspace-scoped:
```bash
agy plugin install ./openclaw-ops
```
Copies this directory to `.agents/plugins/openclaw-ops/` in the current workspace.

Global:
```bash
agy plugin install --global ./openclaw-ops
```
Copies this directory to `~/.gemini/config/plugins/openclaw-ops/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/openclaw-ops
