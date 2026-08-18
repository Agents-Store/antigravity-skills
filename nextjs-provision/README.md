# nextjs-provision (Antigravity plugin)

Next.js provisioning plugin. Set up shadcn/ui and shadcn studio — component installation, theme configuration, MCP server setup, project scaffolding, and multi-registry component search across 260+ registries from the official directory.

## Install

Workspace-scoped:
```bash
agy plugin install ./nextjs-provision
```
Copies this directory to `.agents/plugins/nextjs-provision/` in the current workspace.

Global:
```bash
agy plugin install --global ./nextjs-provision
```
Copies this directory to `~/.gemini/config/plugins/nextjs-provision/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:


## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/nextjs-provision
