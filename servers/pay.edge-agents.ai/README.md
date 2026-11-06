# pay.edge-agents.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/pay.edge-agents.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://pay.edge-agents.ai/mcp` | 7 | [`56dca697f361`](0833964f1b6804488525.json) | 2026-09-14 |

## Tools at `https://pay.edge-agents.ai/mcp`

- `edge_get_free_sample`: `Fetch a free, illustrative sample of a service's output so the response shape and evidence style can be inspected before paying. The sample…`
- `edge_get_report_terms`: `Read the live x402 payment terms for a service's report: the price, and one offer per settlement rail, exactly as the paid endpoint issues…`
- `edge_get_service`: `Look up one service by its id and return its full public record: what it produces, its price, its freshness target, its output schema versi…`
- `edge_list_families`: `List the families the catalogue is organised into, with a service count for each. Use this to browse when a keyword search is too narrow, o…`
- `edge_list_products`: `List the packaged products, each of which composes several specialist services into one buyer outcome, with its free sample and its represe…`
- `edge_search_services`: `Find intelligence services by keyword. Returns id, name, description, family and price for each match. Start here when you know what eviden…`
- `edge_service_health`: `Report per-service availability and data freshness. Call this when a purchase matters and staleness would change the decision: a service ca…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://pay.edge-agents.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
