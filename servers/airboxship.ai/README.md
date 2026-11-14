# airboxship.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/airboxship.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://airboxship.ai/mcp-public` | 3 | [`c5dd0a91a673`](af5c793e229b96d143a5.json) | 2026-11-14 |

## Tools at `https://airboxship.ai/mcp-public`

- `find_pickup_hubs`: `Find nearby USPS Post Offices and Smart Lockers for package pickup/drop-off. Returns each location's id, name, type, address and distance i…`
- `get_shipping_rates`: `Get shipping rates (postage cost and delivery time) for mailing a package with USPS or UPS home delivery, between two US addresses. Returns…`
- `track_package`: `Look up the current status of a USPS package by its tracking number. Returns the status, USPS's one-line summary, the expected delivery dat…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://airboxship.ai/mcp-public"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
