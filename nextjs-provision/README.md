# nextjs-provision (Antigravity skills)

Next.js provisioning plugin. Set up shadcn/ui and shadcn studio — component installation, theme configuration, MCP server setup, project scaffolding, and multi-registry component search across 30+ free community registries.

## Install

Project-scoped:
```bash
cp -r skills/* /path/to/your-project/.agent/skills/
```

User-global:
```bash
cp -r skills/* ~/.gemini/antigravity/skills/
```

## Skills (8)

- `nextjs-provision-component-registry` — Browse, search, install, and use shadcn/ui and shadcn studio components, blocks, and templates. This skill should be used when the user asks to "install a shadcn component", "add a button", "list shadcn blocks", "find a form block", "browse shadcn studio components", "add a card component", "install a navigation block", "what components are available", "write code with shadcn components", "use Button component", "render shadcn component as link", "Button as a link", "shadcn component patterns", or needs to discover, install, or use UI components from shadcn registries correctly.

- `nextjs-provision-component-search` — Search and install UI components from 30+ free community shadcn registries. This skill should be used when the user asks to "search for shadcn components", "find a calendar component", "browse community registries", "install from magicui", "what shadcn registries are available", "add animated components", "search for a date picker", "find UI blocks for landing page", "install from aceternity", "what community components exist", or needs to discover and install components from community registries beyond the standard shadcn/ui and shadcn studio registries.

- `nextjs-provision-examples` — End-to-end scenario walkthroughs for setting up Next.js projects with shadcn/ui and shadcn studio. This skill should be used when the user asks for "shadcn setup walkthrough", "how to set up a project with shadcn from scratch", "add shadcn to existing project example", "full shadcn setup guide", "shadcn studio tutorial", "step-by-step shadcn setup", or needs a complete example of provisioning a Next.js project with shadcn components.

- `nextjs-provision-mcp-tools` — Set up and use shadcn MCP servers for AI-assisted component discovery and installation. This skill should be used when the user asks about "shadcn MCP", "shadcn MCP server", "set up shadcn MCP for Claude", "component MCP tools", "Jpisnice shadcn MCP", "shadcn-ui-mcp-server", "AI component installation", or needs to configure MCP servers for shadcn/ui component work.

- `nextjs-provision-project-scaffolding` — Scaffold Next.js projects with shadcn/ui templates, starter kits, and component architecture patterns. This skill should be used when the user asks to "scaffold a project", "use a shadcn template", "project structure with shadcn", "component organization", "set up a dashboard template", "starter kit for shadcn", "how to organize shadcn components", or needs guidance on organizing a Next.js project with shadcn/ui component architecture.

- `nextjs-provision-setup` — Set up shadcn/ui and shadcn studio in a Next.js project. This skill should be used when the user asks to "set up shadcn", "install shadcn/ui", "initialize shadcn", "configure shadcn studio", "add shadcn to my project", "set up component library", "init shadcn in next.js", or needs to initialize a Next.js project for shadcn/ui component development.

- `nextjs-provision-theme-configuration` — Configure themes, CSS variables, colors, fonts, and dark mode for shadcn/ui and shadcn studio. This skill should be used when the user asks to "set up a theme", "customize shadcn colors", "add dark mode", "change shadcn theme", "use shadcn theme generator", "configure CSS variables for shadcn", "install a shadcn studio theme", "customize fonts", "brand colors for shadcn", or needs to design and apply visual themes to their shadcn/ui project.

- `nextjs-provision-troubleshoot` — Diagnose and fix common shadcn/ui and shadcn studio setup issues, dependency conflicts, and configuration problems. This skill should be used when the user encounters "shadcn install error", "components.json error", "tailwind not working with shadcn", "shadcn component not rendering", "CSS variables not applied", "shadcn studio registry error", "dependency conflict", "cn() not found", or needs to debug problems with their shadcn/ui setup.


## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/nextjs-provision
