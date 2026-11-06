# www.deepinquiry.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.deepinquiry.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.deepinquiry.ai/mcp` | 3 | [`b8f4e07e9bff`](cd9b9f0926a349bf4c17.json) | 2026-10-16 |

## Tools at `https://www.deepinquiry.ai/mcp`

- `get_fact`: `Fetch one fact by its numeric id, with its source groups.`
- `random_fact`: `Fetch one random approved fact.`
- `search_facts`: `Semantic search over DeepInquiry verified facts. Returns the closest facts with their sources, tier, score and signature.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.deepinquiry.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
