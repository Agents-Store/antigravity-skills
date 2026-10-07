# vaultwarden-dev (Antigravity plugin)

Vaultwarden dev plugin for Agents Store. Script and integrate a self-hosted Vaultwarden (Bitwarden-compatible) server: what the client API can and cannot do under end-to-end encryption, the identity token flows, organization member management, the /admin panel API, the Bitwarden CLI (bw, bw serve), python-vaultwarden and Terraform, client/server version compatibility, troubleshooting, and a guard hook that asks before a command prints decrypted secrets into the chat. File-based knowledge, no MCP, no stored credentials.

## Install

Workspace-scoped:
```bash
agy plugin install ./vaultwarden-dev
```
Copies this directory to `.agents/plugins/vaultwarden-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./vaultwarden-dev
```
Copies this directory to `~/.gemini/config/plugins/vaultwarden-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/vaultwarden-dev
