# compare.ac: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/compare.ac.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://compare.ac/api/mcp` | 4 | [`8f5b0a8dae67`](1cf28775fc4a4e235114.json) | 2026-11-27 |

## Tools at `https://compare.ac/api/mcp`

- `find_air_conditioners`: `US air conditioners and heat pumps in stock at a tracked store today, cheapest first: window units, portables, through-the-wall units and m…`
- `find_space_heaters`: `US electric space heaters in stock at a tracked store today, cheapest first, with each one's wattage, voltage, type (ceramic, fan, oil-fill…`
- `get_air_conditioner`: `Everything compare.ac holds on one US air conditioner, mini split or heat pump, found by its model number (e.g. "LW1022RD", "DIY-12-HP-WM-1…`
- `size_air_conditioner`: `Calculates what size air conditioner a room needs: the cooling capacity in BTU per hour for a room of a given floor area in square feet, on…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://compare.ac/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
