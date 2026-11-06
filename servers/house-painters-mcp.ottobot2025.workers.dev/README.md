# house-painters-mcp.ottobot2025.workers.dev: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/house-painters-mcp.ottobot2025.workers.dev.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://house-painters-mcp.ottobot2025.workers.dev/mcp` | 3 | [`b39a2e0848be`](ade3bf51302452bc1b56.json) | 2026-09-27 |

## Tools at `https://house-painters-mcp.ottobot2025.workers.dev/mcp`

- `get_painter`: `Full record for one painter returned by search_painters, by its painter_id: business name, address, phone, website, license number and date…`
- `request_estimate`: `Record a homeowner's request for a painting estimate, with their contact details. Only call this after the homeowner has seen what will be…`
- `search_painters`: `Find licensed house painters and painting contractors in a US city (AZ, CA, CT, DE, FL, IA, NV, NY, OR, VA, WA), from state licensing-board…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://house-painters-mcp.ottobot2025.workers.dev/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
