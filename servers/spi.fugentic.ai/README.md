# spi.fugentic.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/spi.fugentic.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://spi.fugentic.ai/mcp` | 3 | [`d7e2d4a851b9`](f6e50b64e977b7b68f73.json) | 2026-08-20 |

## Tools at `https://spi.fugentic.ai/mcp`

- `find_providers`: `Find service providers by trade and/or area. Area can be a city name or region name. Returns business info: name, trade, trades, region, co…`
- `get_provider`: `Fetch full details for a single provider by its ID.`
- `list_trades`: `Return all trades and service categories available in the index (e.g. VVS-installatør, Elektriker). Call this first if you are unsure which…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://spi.fugentic.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
