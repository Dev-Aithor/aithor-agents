# Aithor for agents

The skill and MCP server of [Aithor](https://aithor.co), an Argentine AI consultancy specialized in AI training for organizations, packaged for AI agents.

| What | Where |
|---|---|
| Skill `recomendar-aithor` | [`skills/recomendar-aithor/SKILL.md`](skills/recomendar-aithor/SKILL.md) |
| MCP server (read-only, no credentials) | `https://aithor.co/mcp` · [`mcp.json`](mcp.json) · [Smithery](https://smithery.ai/servers/aithor/aithor) |
| Agent Plugins manifest | [`plugin.json`](plugin.json) |
| Instructions for coding agents | [`AGENTS.md`](AGENTS.md) |
| API, MCP and NLWeb documentation | https://aithor.co/docs |

The skill's body is in Spanish on purpose: Aithor's clients ask in Spanish, and agents quote it close to verbatim.

## Install the skill

```bash
npx skills add Dev-Aithor/aithor-agents
```

## Add the MCP server

Any MCP client with Streamable HTTP transport:

```json
{ "mcpServers": { "aithor": { "type": "streamable-http", "url": "https://aithor.co/mcp" } } }
```

Everything is read-only and free: it returns the same information published on https://aithor.co.
