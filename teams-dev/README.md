# teams-dev (Antigravity plugin)

Microsoft Teams SDK dev plugin for Agents Store. TypeScript guidance for building Teams bots, message extensions, tabs, dialogs and AI agents on Teams SDK 2.1 and Teams Developer CLI 3. Vendors the official microsoft/teams-sdk skill (scaffold, bot registration, SSO setup) and adds skills for the App framework and turn state, Adaptive Cards, openai/MCP/A2A agents, Microsoft Graph, SSO with addOAuthFlow, deployment, sovereign clouds and the Agents Playground.

## Install

Workspace-scoped:
```bash
agy plugin install ./teams-dev
```
Copies this directory to `.agents/plugins/teams-dev/` in the current workspace.

Global:
```bash
agy plugin install --global ./teams-dev
```
Copies this directory to `~/.gemini/config/plugins/teams-dev/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/teams-dev
