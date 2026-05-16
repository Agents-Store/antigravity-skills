# nocodb-dev (Antigravity skills)

NocoDB schema development plugin. Full Meta API v3 coverage — tables, fields (30+ types), views, filters, sorts, hooks (HookV3), comments, scripts, dashboards & widgets, workflows, plus workspaces / members / teams / tokens. Bundles both Data API and Meta API OpenAPI specs.

## Install

Project-scoped:
```bash
cp -r skills/* /path/to/your-project/.agent/skills/
```

User-global:
```bash
cp -r skills/* ~/.gemini/antigravity/skills/
```

## Skills (12)

- `nocodb-dev-api-reference` — NocoDB REST API reference for schema-development work. Loaded only on explicit cite. Use when:
- "NocoDB REST API"
- "API endpoints for tables/fields/views"
- "create a table via API"
- "what's in the OpenAPI spec"
- "Meta API endpoints"
- "field type schemas"
- "Hook v3 payload"
- "dashboard / widget API"

- `nocodb-dev-cli-reference` — NocoDB `nc` CLI reference — schema-focused commands for tables, fields, views, links, hooks. Loaded only on explicit cite. Use when:
- "nc CLI commands"
- "NocoDB CLI schema commands"
- "how do I create a table from the CLI"
- "nc field:create reference"
- "NocoDB agent-skills CLI"

- `nocodb-dev-dashboards` — Create and manage NocoDB Dashboards and Widgets via Meta API v3. Use when:
- "create a dashboard"
- "add a chart / metric / KPI widget"
- "list widgets on a dashboard"
- "fetch widget data"
- "update a dashboard"
- "delete a widget"

- `nocodb-dev-examples` — End-to-end NocoDB schema-development walkthroughs. Use when:
- "show me a schema example"
- "how do I build a CRM in NocoDB?"
- "e-commerce schema example"
- "schema design walkthrough"
- "NocoDB dev scenarios"

- `nocodb-dev-field-management` — Create, update, and delete NocoDB fields across all 30 supported types — text, numeric, date, select, attachment, JSON, geometry, links, lookup, rollup, formula, button, barcode/QR, system fields. Use when:
- "add a field"
- "create a column"
- "rename a field"
- "change field type"
- "delete a column"
- "add a formula"
- "set up lookup or rollup"
- "link two tables"

- `nocodb-dev-mcp-patterns` — NocoDB MCP tools usable for schema-development work. Use when:
- "what MCP tools can I use for schema?"
- "how do I discover NocoDB structure?"
- "MCP for nocodb-dev"
- "can MCP create tables?"
- "NocoDB MCP discovery"

- `nocodb-dev-setup` — Verify NocoDB connection for schema-development work — both transports (MCP + CLI/API). Use when:
- "check NocoDB dev setup"
- "verify NocoDB API access"
- "is the nc CLI working?"
- "can I modify schema?"
- "test NocoDB MCP connection"

- `nocodb-dev-table-management` — Create, update, rename, duplicate, and delete NocoDB tables. Use when:
- "create a new NocoDB table"
- "rename a table"
- "delete a NocoDB table"
- "set the display field"
- "duplicate a table"
- "add a table with initial fields"

- `nocodb-dev-troubleshoot` — Diagnose schema-side NocoDB errors — read-only fields, type-change rejections, broken Lookups, formula errors, view config validation, version mismatches. Use when:
- "field type change rejected"
- "Lookup not working"
- "formula returns ERR"
- "cannot delete table"
- "Kanban not grouping"
- "schema cache stale"
- "NocoDB version too old"

- `nocodb-dev-view-management` — Create, configure, and delete NocoDB views — Grid, Form, Gallery, Kanban, Calendar, Map. Use when:
- "create a kanban view"
- "add a calendar view"
- "build a form for intake"
- "make a gallery of products"
- "set up filters on a view"
- "delete a view"
- "show / hide columns on a view"

- `nocodb-dev-webhooks` — Configure NocoDB webhooks (HookV3) — triggers, conditions, and notification targets (URL, Email, Messaging, Script). Use when:
- "add a webhook"
- "fire a Slack message on insert"
- "send email when a record changes"
- "trigger n8n on update"
- "list webhooks on a table"
- "delete a hook"

- `nocodb-dev-workflows` — List, execute, and inspect NocoDB Workflows (the platform's built-in automation engine) via Meta API v3. Use when:
- "list NocoDB workflows"
- "execute a workflow"
- "view workflow execution"
- "trigger workflow on demand"
- "fetch execution results"


## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/nocodb-dev
