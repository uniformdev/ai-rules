# Cursor Marketplace – AI Rules

This repository is a **Cursor marketplace**: a multi-plugin repo that can be submitted to the Cursor marketplace so others can install the plugins.

## Structure

```
cursor-marketplace/
├── .cursor-plugin/
│   └── marketplace.json       # Marketplace manifest (lists plugins)
├── uniform-rules/             # Plugin: Uniform CMS rules
│   ├── .cursor-plugin/
│   │   └── plugin.json
│   ├── rules/
│   │   ├── uniform.mdc
│   │   ├── uniform-sdk.mdc
│   │   ├── uniform-sveltekit.mdc
│   │   ├── uniform-next-app-router.mdc
│   │   ├── uniform-next-page-router.mdc
│   │   └── uniform-mesh.mdc
│   └── README.md
├── enterprise-toolkit/        # Plugin: Security, compliance, automation
│   ├── .cursor-plugin/
│   │   └── plugin.json
│   ├── rules/
│   ├── skills/
│   ├── agents/
│   ├── commands/
│   ├── hooks/
│   ├── .mcp.json
│   ├── assets/
│   ├── scripts/
│   └── README.md
└── README.md
```

## Plugins

| Plugin              | Description |
|---------------------|-------------|
| **uniform-rules**   | Uniform CMS rules for compositions, components, patterns, SDK, SvelteKit, Next.js, Mesh. |
| **enterprise-toolkit** | Rules, skills, agents, commands, hooks, and optional MCP for security, compliance, and automation. |

## Submitting to the Cursor marketplace

1. Push this repo (or the `cursor-marketplace` folder as its own repo) to a **public** Git host.
2. Go to [cursor.com/marketplace/publish](https://cursor.com/marketplace/publish) and submit the repository URL.
3. Ensure:
   - Each plugin has a valid `.cursor-plugin/plugin.json` with a unique `name` (lowercase, kebab-case).
   - All rules/skills/agents/commands have proper frontmatter.
   - Paths in manifests are relative and valid.
   - You have tested the plugins locally.

## Local use

To use as a local marketplace or single plugin:

- **Multi-plugin**: Point Cursor at the root of `cursor-marketplace` (where `.cursor-plugin/marketplace.json` lives).
- **Single plugin**: Point Cursor at `cursor-marketplace/uniform-rules` or `cursor-marketplace/enterprise-toolkit`.

## License

See repository license. Plugin manifests may specify their own license.
