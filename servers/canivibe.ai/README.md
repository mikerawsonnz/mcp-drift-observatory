# canivibe.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/canivibe.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://canivibe.ai/mcp` | 2 | [`f6fa9f430280`](a3f6f5a9d86e6fdf3a53.json) | 2026-08-20 |

## Tools at `https://canivibe.ai/mcp`

- `ai_provider_status`: `Get the live status of AI coding providers (Claude, OpenAI, Copilot, Cursor, OpenRouter and more). Returns status, how long each provider h…`
- `check_provider_health`: `Check whether one or more AI coding providers are healthy enough to use right now. Returns healthy=true only when every requested provider…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://canivibe.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
