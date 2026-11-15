# stack-ads (Antigravity plugin)

Paid advertising stack for any project. Researches the product and its market, derives targeting, writes ad copy, generates images, video and voice-over, launches paused campaigns on Google Ads, Meta and TikTok from a reviewed dry-run plan with budget ceilings and a rollback ledger, and reports results. Walks the user through obtaining every key. Integrates Google Ads, Search Console, Meta, TikTok, Firecrawl, Apify, DataForSEO, OpenAI, Gemini and fal.ai via MCP and one dependency-free toolkit.

## Install

Workspace-scoped:
```bash
agy plugin install ./stack-ads
```
Copies this directory to `.agents/plugins/stack-ads/` in the current workspace.

Global:
```bash
agy plugin install --global ./stack-ads
```
Copies this directory to `~/.gemini/config/plugins/stack-ads/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## MCP servers

Configured in `mcp_config.json`. Required environment variables:

- `APIFY_TOKEN`
- `DATAFORSEO_PASSWORD`
- `DATAFORSEO_USERNAME`
- `FIRECRAWL_API_KEY`
- `GOOGLE_APPLICATION_CREDENTIALS`
- `GOOGLE_CLOUD_PROJECT`
- `META_ACCESS_TOKEN`

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/stack-ads
