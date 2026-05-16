# dokploy-dev (Antigravity skills)

Dokploy self-hosted PaaS development plugin. Deploy applications, provision databases (Postgres, MySQL, MariaDB, MongoDB, Redis, LibSQL), manage domains, Docker Compose stacks, backups, and server operations via the official @dokploy/mcp server (500+ tools across 49 categories), 463 REST API endpoints, and CLI.

## Install

Project-scoped:
```bash
cp -r skills/* /path/to/your-project/.agent/skills/
```

User-global:
```bash
cp -r skills/* ~/.gemini/antigravity/skills/
```

## Skills (6)

- `dokploy-dev-api-reference` — This skill should be used when making direct HTTP/curl calls to the Dokploy API, looking up endpoint parameters, or building integrations that bypass the MCP server. Triggers: "dokploy API", "curl dokploy", "REST endpoint", "HTTP request to dokploy".
- `dokploy-dev-cli-recipes` — This skill should be used when running Dokploy operations from the terminal, deploying via CLI, managing environment variables with env push/pull, or provisioning databases via command line. Triggers: "dokploy cli", "dokploy command", "env push", "env pull", "dokploy deploy cli".
- `dokploy-dev-examples` — This skill should be used when learning how to deploy apps, provision databases, or set up Docker Compose stacks on Dokploy. Provides end-to-end workflow walkthroughs. Triggers: "dokploy example", "how to deploy on dokploy", "dokploy tutorial", "dokploy walkthrough", "show me how to use dokploy".
- `dokploy-dev-mcp-patterns` — This skill should be used when deploying applications, managing projects, provisioning databases, configuring domains, working with Docker Compose, or performing any Dokploy operation via MCP tools. Triggers: "deploy app", "create project", "add domain", "provision database", "dokploy compose", "manage dokploy".
- `dokploy-dev-setup` — This skill should be used when verifying Dokploy MCP connection, CLI installation, and API access. Use when user says "set up dokploy", "verify dokploy connection", "check dokploy", "test dokploy access", or enables the dokploy-dev plugin for the first time.
- `dokploy-dev-troubleshoot` — This skill should be used when diagnosing Dokploy deployment failures, domain issues, database connection problems, or Docker/Traefik errors. Use when a deployment fails, domain is not resolving, database cannot connect, app returns 502, or MCP tools return errors. Triggers: "dokploy error", "deployment failed", "domain not working", "502 bad gateway", "database connection refused", "dokploy debug".

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/dokploy-dev
