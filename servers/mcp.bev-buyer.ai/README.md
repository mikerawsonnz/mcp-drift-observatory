# mcp.bev-buyer.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.bev-buyer.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.bev-buyer.ai/mcp` | 9 | [`70c465df6d89`](76770373d48a68fc84d5.json) | 2026-10-01 |

## Tools at `https://mcp.bev-buyer.ai/mcp`

- `accept_offer`: `Accept one offer and place the order through the Bourse. Accepting is one x402 paid call (HTTP 402 with the payment offer until paid): it s…`
- `compare_drinks`: `Compare two to ten products side by side, field by field, each value with its source page.`
- `create_order_intent`: `Place an order intent for one to ten records (quantity, delivery market, optional date and note, the buyer's organisation and email). The B…`
- `find_producer`: `Find a maker and its products across every open node, with the maker's name as each source wrote it.`
- `get_offers`: `Read the makers' offers on an order intent, and the order once placed. By the buyer's email given on create_order_intent.`
- `get_order_route`: `Get the maker's or distributor's trade channel to order a product, as the record states it. Never a consumer channel.`
- `get_record`: `Read one product in full by record_id: every field with its source page, reader and state; its CUVEE; its claim status; the signed record (…`
- `list_nodes`: `List the countries on the record: each node's door, languages, state and, for an open node, its counts.`
- `search_drinks`: `Find beers, wines, spirits, ciders and ready-to-drink drinks by name, style, origin or category across every open country node. Returns rec…`

## Changes

- 2026-10-01: [annotation changed, field changed, schema changed](../../deltas/2026-10-01/76770373d48a68fc84d5.json): `28 field(s) changed`
- 2026-09-29: [count changed, tool added](../../deltas/2026-09-29/76770373d48a68fc84d5.json): `3 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.bev-buyer.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
