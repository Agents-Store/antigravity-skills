# stack-flask-sqlalchemy (Antigravity plugin)

Flask + SQLAlchemy architecture plugin. How the application factory, the Flask-SQLAlchemy session, Alembic migrations and Jinja2 templates fit together: where db is created, the app context, the transaction boundary, expire_on_commit, N+1 at the route-to-template edge, and a full-feature recipe. Tool knowledge comes from its dependencies flask-dev and sqlalchemy-dev.

## Install

Workspace-scoped:
```bash
agy plugin install ./stack-flask-sqlalchemy
```
Copies this directory to `.agents/plugins/stack-flask-sqlalchemy/` in the current workspace.

Global:
```bash
agy plugin install --global ./stack-flask-sqlalchemy
```
Copies this directory to `~/.gemini/config/plugins/stack-flask-sqlalchemy/` instead.

## Workflows (UNVERIFIED)

The `workflows/*.md` directory convention is **not confirmed by official Antigravity documentation** as of 2026-08-17. If workflows aren't picked up automatically after install, paste their content manually via the editor's "+ Workspace" button.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/stack-flask-sqlalchemy
