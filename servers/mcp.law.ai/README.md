# mcp.law.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.law.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.law.ai` | 5 | [`cb1fe7c5421a`](84043d90c69400969f98.json) | 2026-08-20 |

## Tools at `https://mcp.law.ai`

- `find_lawyer_by_name`: `Look up a lawyer by name to verify they exist and are licensed.`
- `get_jurisdictions`: `List US states with lawyer counts.`
- `get_lawyer_profile`: `Get full profile for a specific lawyer by their Law.AI ID.`
- `get_practice_areas`: `List all practice areas with lawyer counts.`
- `search_lawyers`: `Search verified lawyer profiles by practice area, state, city, and bar status.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.law.ai"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
