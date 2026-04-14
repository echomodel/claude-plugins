# echomodel Claude Plugins

Claude Code plugin marketplace for the [echomodel](https://github.com/echomodel) org.

## Installation

```bash
claude plugin marketplace add https://github.com/echomodel/claude-plugins.git
```

After that the marketplace is registered locally as `echomodel`.

## Available plugins

| Plugin | Description | Install |
|--------|-------------|---------|
| [claude-coding](https://github.com/echomodel/claude-coding) | Coding agent with privacy-gated commits, session lifecycle, and skill composition | `claude plugin install claude-coding@echomodel --scope user` |
| [plugin-creator](https://github.com/echomodel/claude-plugin-creator) | Scaffold Claude Code plugins with self-installing local MCP servers and guide ongoing plugin authorship. Install at `--scope project` in a plugin's repo so its patterns guidance is loaded only when working on that plugin. | `claude plugin install plugin-creator@echomodel --scope project` |
| [gapp](https://github.com/echomodel/gapp) | Deploy Python MCP servers to Cloud Run with guided lifecycle, CI/CD, custom domains, and secret management | `claude plugin install gapp@echomodel --scope user` |

## Plugin architecture docs

Architecture and design patterns for building Claude Code plugins that bundle local MCP servers and compose skills live in the [claude-plugin-creator](https://github.com/echomodel/claude-plugin-creator) repo:

- [Plugin patterns](https://github.com/echomodel/claude-plugin-creator/blob/main/docs/plugin-patterns.md) — self-installing MCP servers, install-pattern variants and antipattern, plugin-as-orchestration via the bundling guarantee, MCP orchestration

## Prerequisites

Each plugin may have its own prerequisites. See the plugin's README for details.
