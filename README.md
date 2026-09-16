# Era Claude Code Plugin

Connect Claude Code to [Era](https://console.era.eon.io) via this plugin. Bundles the Era MCP server so an agent can sign in, provision a synthetic design partner, and manage its connector fleet without leaving Claude Code.

## Capabilities

- **Era MCP server** — sign in (or complete OAuth), list the connectors a design partner can be built across, provision one, add systems to it, watch its build, rotate or scope its tokens, check usage, and remove it — all as MCP tools.
- **`era` skill** — teaches Claude Code what Era is and how to work in one: signing in, provisioning a synthetic company, reaching its systems over REST or as custom MCP servers, and investigating across them.

## Installation

Run inside Claude Code:

```
/plugin marketplace add eon-io/claude-code-era-plugin
/plugin install era@era-eon-io
```

## MCP Server

The plugin connects to `https://console.era.eon.io/mcp` via HTTP. Authentication is handled by Era's own sign-in flow.

## Local Development

```bash
claude --plugin-dir .
```

Run `/reload-plugins` inside Claude Code after making local edits.

## Links

- [Era](https://console.era.eon.io)
- [Eon](https://eon.io)

## License

Licensed under the [Apache License, Version 2.0](LICENSE). See [NOTICE](NOTICE) for attribution and the scope of the license — the Era service, API, and trademarks are not covered.
