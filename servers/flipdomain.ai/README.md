# flipdomain.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/flipdomain.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://flipdomain.ai/mcp` | 4 | [`2138aa04f05a`](f5c6ea67b3aa16dcd250.json) | 2026-08-20 |

## Tools at `https://flipdomain.ai/mcp`

- `get_domain`: `Get the current asking price and buyer paths for an exact domain in the live sale catalog.`
- `list_clearance_domains`: `List time-sensitive renewal-clearance domains by maximum price, category, or TLD.`
- `make_offer`: `Submit a genuine USD offer for a saleable domain. The seller receives it through the live offer pipeline.`
- `search_domains`: `Search the live FlipDomain.ai portfolio by keyword, category, TLD, collection, and price. Returns saleable domains only.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://flipdomain.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
