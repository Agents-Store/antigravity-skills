# dify-dev (Antigravity skills)

Dify API dev plugin for Agents Store. Complete coverage of the Dify App Service API (chat, completion, workflows, conversations, files, audio, annotations) and the Knowledge Base / Datasets API — auth, endpoints, streaming events, curl examples, and troubleshooting.

## Install

Project-scoped:
```bash
cp -r skills/* /path/to/your-project/.agent/skills/
```

User-global:
```bash
cp -r skills/* ~/.gemini/antigravity/skills/
```

## Skills (9)

- `dify-dev-annotations` — This skill should be used when the user asks to "list/create/update/delete Dify annotations", "call /apps/annotations", "set up Dify annotation reply", "enable annotation reply", "disable annotation reply", or "check annotation reply status". Covers the annotation (curated Q&A) subsystem.

- `dify-dev-chat-completion` — This skill should be used when the user asks to "send a chat message to Dify", "call /chat-messages", "use the Dify completion API", "/completion-messages", "stream a Dify chat response", "stop Dify generation", "get suggested questions", or "submit message feedback / like a message". Covers conversational (chat/agent/ chatflow) and stateless (completion) message sending.

- `dify-dev-conversations` — This skill should be used when the user asks to "list Dify conversations", "get conversation history", "list messages in a Dify conversation", "rename a Dify conversation", "delete a conversation", or "get/update Dify conversation variables". Covers chat-history management for chat/agent/chatflow apps.

- `dify-dev-examples` — This skill should be used when the user asks for a "full Dify example", "end-to-end Dify integration", "how do I build a chatbot with Dify", "complete workflow example", "Dify RAG example", or wants a working, copy-paste walkthrough that strings multiple Dify API calls together.

- `dify-dev-files-audio` — This skill should be used when the user asks to "upload a file to Dify", "call /files/upload", "send an image to a Dify app", "transcribe audio with Dify", "/audio-to-text", "Dify text to speech", or "/text-to-audio". Covers file upload for multimodal input and the speech endpoints.

- `dify-dev-knowledge-base` — This skill should be used when the user asks to work with Dify "knowledge base", "datasets API", "create a dataset", "upload a document to Dify", "add documents to a knowledge base", "segments / chunks", "retrieve from a Dify knowledge base", "test retrieval", or RAG ingestion. Covers the standalone Knowledge Base / Datasets API.

- `dify-dev-setup` — This skill should be used when the user asks how to "connect to the Dify API", "authenticate with Dify", "get a Dify API key", "what is the Dify base URL", "blocking vs streaming in Dify", "the Dify user field", "send files to a Dify app", or needs the app metadata endpoints (/info, /parameters, /meta, /site). Foundation for every other Dify API call.

- `dify-dev-troubleshoot` — This skill should be used when a Dify API call fails or behaves unexpectedly — "Dify 401 / 404 / 429 error", "Dify conversation not found", "Dify blocking timeout", "Dify rate limit", "why is my Dify conversation empty", "Dify user mismatch", or "Dify file upload not working". Error codes, limits, and common pitfalls.

- `dify-dev-workflows` — This skill should be used when the user asks to "run a Dify workflow", "call /workflows/run", "execute a Dify workflow app via API", "get a workflow run result", "list Dify workflow logs", "stop a Dify workflow task", or work with Chatflow/Workflow node events. Covers Workflow-type apps (no conversation wrapper).


## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/dify-dev
