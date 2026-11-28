# 48.brainy.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/48.brainy.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://48.brainy.ae/mcp` | 5 | [`8535ba9a5185`](469089a5676175c4aa62.json) | 2026-11-28 |

## Tools at `https://48.brainy.ae/mcp`

- `compare_ai_seat_costs`: `Compare 12-month AI seat and automation costs in USD and AED. Estimates use the AED catalogue price. Token counts per run are optional.`
- `estimate_diagnosis`: `Compare interview schedules and see what the free diagnosis includes and who qualifies.`
- `list_automations`: `List catalogue automations, prices and estimated delivery days in UAE or Spain.`
- `receipts_to_spreadsheet_free`: `Get the free receipt-to-Excel page, its limits and privacy details. Direct users to upload on the page.`
- `request_free_diagnosis`: `Get the conditions and a pre-filled WhatsApp link for the user to open.`

## Changes

- 2026-11-28: [count changed, tool added](../../deltas/2026-11-28/469089a5676175c4aa62.json): `1 tool(s) added`
- 2026-11-25: [count changed, tool added](../../deltas/2026-11-25/469089a5676175c4aa62.json): `1 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://48.brainy.ae/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
