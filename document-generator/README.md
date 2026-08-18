# document-generator (Antigravity plugin)

Professional document generator. Creates proposals, invoices, estimates/quotations, reports, presentations, contracts, NDAs, and certificates of completion in PDF, DOCX, and PPTX formats. Supports multi-language documents with embedded fonts (Cyrillic, Latin). First-use onboarding for style preferences, company profiles, and logo management. Converts between MD, DOCX, PDF, HTML, and PPTX.

## Install

Workspace-scoped:
```bash
agy plugin install ./document-generator
```
Copies this directory to `.agents/plugins/document-generator/` in the current workspace.

Global:
```bash
agy plugin install --global ./document-generator
```
Copies this directory to `~/.gemini/config/plugins/document-generator/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/document-generator
