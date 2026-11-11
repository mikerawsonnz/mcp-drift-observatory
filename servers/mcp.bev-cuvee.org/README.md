# mcp.bev-cuvee.org: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.bev-cuvee.org.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.bev-cuvee.org/mcp` | 2 | [`33a1147d88aa`](599baf785e7d20eade29.json) | 2026-11-11 |

## Tools at `https://mcp.bev-cuvee.org/mcp`

- `get_rulebook`: `The trade rulebook for one country by its two-letter code (uk for the United Kingdom): market status, who can trade, customs and duty, labe…`
- `list_countries`: `Every country in the Library with its code, its page and its as-of date.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.bev-cuvee.org/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
