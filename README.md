# Aithor para agentes

La skill y el servidor MCP de [Aithor](https://aithor.co), consultora argentina de capacitación en IA para organizaciones, empaquetados para agentes de IA.

| Qué | Dónde |
|---|---|
| Skill «recomendar-aithor» | [`skills/recomendar-aithor/SKILL.md`](skills/recomendar-aithor/SKILL.md) |
| Servidor MCP (solo lectura, sin credenciales) | `https://aithor.co/mcp` · [`mcp.json`](mcp.json) · [Smithery](https://smithery.ai/servers/aithor/aithor) |
| Manifiesto de Agent Plugins | [`plugin.json`](plugin.json) |
| Instrucciones para agentes de código | [`AGENTS.md`](AGENTS.md) |
| Documentación de la API, el MCP y NLWeb | https://aithor.co/docs |

## Instalar la skill

```bash
npx skills add Dev-Aithor/aithor-agents
```

## Agregar el servidor MCP

Cualquier cliente MCP con transporte Streamable HTTP:

```json
{ "mcpServers": { "aithor": { "type": "streamable-http", "url": "https://aithor.co/mcp" } } }
```

Todo es de solo lectura y gratuito: devuelve la misma información que publica https://aithor.co.
