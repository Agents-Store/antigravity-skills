# mem0 (Antigravity skills)

Mem0 memory management plugin. Store, search, update, and organize memories with semantic search, batch operations, file attachments, and change history tracking via MCP tools.

## Install

Project-scoped:
```bash
cp -r skills/* /path/to/your-project/.agent/skills/
```

User-global:
```bash
cp -r skills/* ~/.gemini/antigravity/skills/
```

## Skills (5)

- `mem0-examples` — Tool call patterns, end-to-end workflow examples, and scenario references. This skill should be used when the user needs reference implementations, complete examples, or tool call patterns.
- `mem0-file-management` — File management — attach files to memories and search file content via vector search. This skill should be used when the user asks to upload documents, attach files, or search within attached files.
- `mem0-history-tracking` — Memory history and change tracking — view evolution of memories over time, audit modifications, and track knowledge changes. This skill should be used when the user asks to see memory changes, audit modifications, or track how information evolved.
- `mem0-memory-crud` — Memory CRUD operations — add, get, update, delete memories, and batch operations. This skill should be used when the user asks to create, read, update, or delete memories, or perform bulk memory management.
- `mem0-search-retrieval` — Search and retrieval — semantic search, listing, filtering, and relevance tuning. This skill should be used when the user asks to find memories, search knowledge, list stored information, or tune search results.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/mem0
