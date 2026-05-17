# payloadcms-dev (Antigravity skills)

PayloadCMS dev plugin for Agents Store. Covers collections, fields, hooks, access control, queries, adapters, Lexical rich text, jobs queue, plugin development, Next.js integration, CLI, migrations, and end-to-end scenarios for TypeScript developers building with Payload v3.

## Install

Project-scoped:
```bash
cp -r skills/* /path/to/your-project/.agent/skills/
```

User-global:
```bash
cp -r skills/* ~/.gemini/antigravity/skills/
```

## Skills (16)

- `payloadcms-dev-access-control` — This skill should be used when the user asks about "Payload access control", "RBAC in Payload", "row-level security", "isAdmin function", "field access control", "global access control", "overrideAccess", "multi-tenant Payload", "filter by user role", "Payload Access function", or needs to decide who can create/read/update/delete documents.
- `payloadcms-dev-adapters` — This skill should be used when the user asks about "Payload database adapter", "Postgres in Payload", "MongoDB Payload setup", "SQLite Payload", "S3 storage adapter", "Cloudflare R2 Payload", "Vercel Blob upload", "Payload email Resend", "Payload Nodemailer SMTP", "Payload transactions", or needs to wire Payload to a database, file storage, or email provider.
- `payloadcms-dev-api-reference` — This skill should be used when the user asks for "PayloadCMS REST endpoint", "Payload curl example", "Payload GraphQL query syntax", "Payload Local API method signature", "Payload login endpoint", "Payload auth headers", or needs the exact HTTP/method signature for a Payload API call.
- `payloadcms-dev-cli-recipes` — This skill should be used when the user asks about "payload migrate", "payload generate:types", "payload generate:importmap", "payload migrate:create", "payload migrate:down", "payload migrate:reset", "payload migrate:refresh", "payload migrate:status", "Payload CLI commands", or needs to run the Payload command-line tool for schema migrations or codegen.
- `payloadcms-dev-cms-migration` — This skill should be used when the user asks to "migrate WordPress to Payload", "move content from Contentful to Payload", "import Strapi data into Payload", "migrate Sanity to PayloadCMS", "Webflow CMS to Payload", "design Payload collections from CMS export", or needs a structured workflow for moving content from another CMS into Payload.
- `payloadcms-dev-collections` — This skill should be used when the user asks to "create a Payload collection", "define a CollectionConfig", "set up an auth collection", "build an upload collection", "add drafts/versions", "configure admin panel for a collection", "enable live preview", "set defaultColumns", or needs to model any content type in PayloadCMS v3.
- `payloadcms-dev-examples` — This skill should be used when the user asks "show me a complete Payload example", "give me a working Payload blog", "Payload ecommerce example", "Payload auth-only API example", "Payload jobs worker example", "Payload multi-tenant example", or wants end-to-end scenario walkthroughs instead of isolated snippets.
- `payloadcms-dev-fields` — This skill should be used when the user asks about "Payload field types", "add a relationship field", "blocks field", "array field", "rich text field", "upload field", "virtual field", "conditional fields", "field validation", "join field", "point/geolocation field", "slug field helper", or needs to design any field inside a PayloadCMS collection or global.
- `payloadcms-dev-hooks` — This skill should be used when the user asks about "Payload hooks", "beforeChange", "afterChange", "afterRead", "beforeDelete", "field hooks", "global hooks", "prevent hook loops", "Next.js revalidation in Payload", "transaction safe hooks", "auto-set author from req.user", or needs to wire up lifecycle automation in PayloadCMS.
- `payloadcms-dev-jobs-queue` — This skill should be used when the user asks about "Payload jobs queue", "Payload background tasks", "Payload workflows", "Payload cron scheduling", "Payload task retries", "Payload runJobs", "Payload autoRun", "queue a job in Payload", or needs to run any background or scheduled work in PayloadCMS.
- `payloadcms-dev-lexical-editor` — This skill should be used when the user asks about "Payload rich text", "Lexical editor in Payload", "custom Lexical feature", "richText blocks", "richText link/upload/relationship", "custom Lexical node", "render Payload Lexical to JSX", "convert Lexical to HTML", or needs to customize the editor inside `richText` fields.
- `payloadcms-dev-nextjs-integration` — This skill should be used when the user asks about "Payload with Next.js", "getPayload in server component", "Payload App Router", "Payload route groups", "Payload live preview Next.js", "revalidate Payload page", "Payload server actions", "Payload draft mode", "Payload Next.js cache", or needs to wire PayloadCMS into a Next.js v14/v15 frontend.
- `payloadcms-dev-plugin-development` — This skill should be used when the user asks to "build a Payload plugin", "create payload-plugin package", "write a Payload plugin from scratch", "add fields via plugin", "preserve hooks in plugin", "publish payload-plugin to npm", "plugin architecture in Payload", or needs to author or maintain a reusable PayloadCMS plugin.
- `payloadcms-dev-queries` — This skill should be used when the user asks about "Payload Local API", "payload.find", "payload.findByID", "where query", "Payload query operators", "depth and populate", "filter Payload by relationship", "sort and paginate Payload results", "Payload REST API query string", "GraphQL queries", or needs to read or write data with Payload.
- `payloadcms-dev-setup` — This skill should be used when the user asks to "install PayloadCMS", "create a Payload project", "set up Payload v3", "scaffold Payload app", "initialize Payload with Next.js", "pick a Payload database adapter", "configure payload.config.ts", or needs to bootstrap a fresh Payload project from zero to a running admin panel.
- `payloadcms-dev-troubleshoot` — This skill should be used when the user asks about "Payload error", "Payload not working", "Payload TypeError", "access bypass in Local API", "Payload hook infinite loop", "Payload transaction rollback", "Cannot find module payload", "Payload import map missing", "Payload type generation fails", "Could not resolve component", or sees a stack trace from Payload they want decoded.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/payloadcms-dev
