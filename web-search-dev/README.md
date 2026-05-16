# web-search-dev (Antigravity skills)

Web search and scraping developer toolkit...

## Install

Project-scoped:
```bash
cp -r skills/* /path/to/your-project/.agent/skills/
```

User-global:
```bash
cp -r skills/* ~/.gemini/antigravity/skills/
```

## Skills (10)

- `web-search-dev-api-reference` — This skill should be used when the user asks for "Firecrawl API endpoints", "Exa REST API", "Perplexity API reference", "Jina API curl examples", "web search API documentation", or needs specific HTTP endpoint details for any of the web search and scraping services.
- `web-search-dev-cli-recipes` — This skill should be used when the user asks about "firecrawl CLI", "jina CLI", "firecrawl command line", "jina command line", "scrape from terminal", "search from shell", or needs ready-to-use CLI commands for web scraping and search.
- `web-search-dev-doc-search` — This skill should be used when the user asks to "find docs", "search documentation", "look up API reference", "find framework docs", "check Next.js docs", "search React docs", "find current docs for a library", or needs to find up-to-date documentation for a framework, library, or service while developing.
- `web-search-dev-examples` — This skill should be used when the user asks for "web search examples", "scraping examples", "show me how to use search tools", "search workflow examples", or needs end-to-end scenario walkthroughs for web search and scraping development tasks.
- `web-search-dev-mcp-patterns` — This skill should be used when the user asks about "web search MCP tools", "which search tools are available", "firecrawl tools", "exa tools", "jina tools", "perplexity tools", "how to use search MCP", "scraping MCP tools", "media search tools", or needs to know which MCP operations are available across web search and scraping services. Also triggers when doing any web research, URL fetching, or page content extraction — including during planning, exploration, or data source analysis.
- `web-search-dev-media-search` — This skill should be used when the user asks to "find images", "search photos", "find stock photos", "search videos", "find media for app", "get stock images", "find pictures for website", or needs to find images, videos, or other media content for their application or website.
- `web-search-dev-sdk-patterns` — This skill should be used when the user asks about "Firecrawl SDK", "Exa SDK", "exa-js", "exa-py", "Perplexity SDK", "Jina SDK", "web search client library", "search npm package", "search Python package", or needs code patterns for integrating web search services into a project.
- `web-search-dev-setup` — This skill should be used when the user asks to "verify web search setup", "check search services", "test firecrawl connection", "test exa connection", "is jina working", "check perplexity MCP", or needs to confirm which web search and scraping services are operational.
- `web-search-dev-troubleshoot` — This skill should be used when the user encounters "search not working", "scrape failing", "firecrawl error", "exa error", "jina error", "perplexity error", "rate limit", "401 unauthorized", "MCP connection failed", or needs to diagnose and fix problems with any web search or scraping service.
- `web-search-dev-web-scraping` — This skill should be used when the user asks to "scrape a website", "extract content from URL", "crawl a site for data", "parse website content", "build a scraper", "extract product data", "scrape for my app", or needs to extract web content for their application or data pipeline. Also use when researching external data sources, analyzing websites for data availability, or fetching page content during planning — any task that involves reading web page content should use MCP scraping tools (firecrawl, jina, exa) instead of basic WebFetch.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/web-search-dev
