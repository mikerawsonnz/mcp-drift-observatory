# beexcellent.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/beexcellent.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://beexcellent.ai/api/mcp/public` | 5 | [`0fcc20fab14d`](fed44102cd8d6f46fdce.json) | 2026-11-05 |

## Tools at `https://beexcellent.ai/api/mcp/public`

- `excellent_help`: `Excellent's own help text (the passages its in-app assistant answers from): how to do a task in Excellent — proposals, e-signed contracts,…`
- `find_event_venues`: `Finds restaurants and venues on Excellent that accept private-event and group-dining inquiries from AI assistants, by the restaurant group'…`
- `search_excellent_pages`: `Search Excellent's published pages: feature pages (what each part of the product does), comparison pages (Excellent vs another events or pr…`
- `send_event_inquiry`: `Sends a private-event or group-dining inquiry, on behalf of the person you are helping, to a venue that accepts inquiries from AI assistant…`
- `start_excellent_workspace`: `Creates a new Excellent workspace filled with sample data (a fictional restaurant group with two venues, bookings, proposals, invoices, sta…`

## Changes

- 2026-11-05: [count changed, tool added](../../deltas/2026-11-05/fed44102cd8d6f46fdce.json): `2 tool(s) added`
- 2026-11-04: [description changed, schema changed](../../deltas/2026-11-04/fed44102cd8d6f46fdce.json): `2 field(s) changed`
- 2026-11-02: [count changed, tool added](../../deltas/2026-11-02/fed44102cd8d6f46fdce.json): `1 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://beexcellent.ai/api/mcp/public"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
