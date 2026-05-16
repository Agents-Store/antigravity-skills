# dify-ops (Antigravity skills)

Dify self-hosted update operations plugin. Pull upstream changes, merge into local dev branch, sync .env variables, detect Docker project names, and rebuild containers for Dify Docker deployments.

## Install

Project-scoped:
```bash
cp -r skills/* /path/to/your-project/.agent/skills/
```

User-global:
```bash
cp -r skills/* ~/.gemini/antigravity/skills/
```

## Skills (4)

- `dify-ops-dify-docker-architecture` — Dify Docker Compose deployment architecture — services, container naming, directory layout, .env.example structure, and Docker project name conventions. Use when working with Dify Docker setup, understanding container services, debugging container issues, or needing to know the Dify directory structure. Triggers on "dify docker", "dify containers", "dify services", "dify architecture", "dify compose".

- `dify-ops-env-sync` — Synchronize .env with .env.example for Dify Docker deployments — detect new variables, add missing ones with default values, preserve existing customizations. Use when syncing env variables, checking for new Dify configuration variables, comparing .env.example vs .env, "env sync", "new env variables", "missing environment variables", or after pulling Dify updates.

- `dify-ops-examples` — End-to-end scenario walkthroughs for updating self-hosted Dify. Use when the user asks for "dify update example", "how to update dify", "show me an update walkthrough", "dify upgrade guide", "step-by-step dify update", or needs a complete example of the update process.

- `dify-ops-update-workflow` — Git workflow for updating self-hosted Dify — fetch upstream, merge main into dev, handle conflicts, checkout specific tags. Use when updating Dify, merging upstream changes, handling merge conflicts in Dify, or switching to a specific Dify version/tag. Triggers on "update dify", "pull dify changes", "merge main into dev", "upgrade dify", "dify version".


## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/dify-ops
