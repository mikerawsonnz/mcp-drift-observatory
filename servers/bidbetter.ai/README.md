# bidbetter.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/bidbetter.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://bidbetter.ai/api/mcp` | 2 | [`55c7273d2d0c`](4912a61ad98f2d37dfb1.json) | 2026-11-04 |

## Tools at `https://bidbetter.ai/api/mcp`

- `list_models`: `Every collector-car model BidBetter publishes a value for, with its median, band, sale count and page URL. Call this first when you are uns…`
- `value_model`: `Median, 25th-75th percentile band and sale count for a specific collector-car model and year range, from completed auction sales. Use for q…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://bidbetter.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
