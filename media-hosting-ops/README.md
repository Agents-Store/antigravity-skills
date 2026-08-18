# media-hosting-ops (Antigravity plugin)

Media hosting operations plugin. Upload images by public URL to MinIO-based media hosting via the uploadImageToMinio MCP tool.

## Install

Workspace-scoped:
```bash
agy plugin install ./media-hosting-ops
```
Copies this directory to `.agents/plugins/media-hosting-ops/` in the current workspace.

Global:
```bash
agy plugin install --global ./media-hosting-ops
```
Copies this directory to `~/.gemini/config/plugins/media-hosting-ops/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/media-hosting-ops
