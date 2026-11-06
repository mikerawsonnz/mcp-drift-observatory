# coreplex.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/coreplex.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://coreplex.ai/api/apps/6a9567482e969b1ab43e0c49/functions/coreplexMcp` | 7 | [`4da4510bb171`](bb6a0d0f9fe0ea79342b.json) | 2026-10-20 |

## Tools at `https://coreplex.ai/api/apps/6a9567482e969b1ab43e0c49/functions/coreplexMcp`

- `compare_prices`: `Other sellers of the exact same item (catalog ID or barcode), lowest first; similar listings kept apart. Example: {"product_url":"https://o…`
- `find_health_products`: `Health products by seller-stated claim (HSA/FSA, USP, NSF, Informed Sport, GMP, ConsumerLab). Example: {"filter":"hsa_fsa","query":"vitamin…`
- `get_passport`: `Brand's own listing, then every store selling it, marked same, likely same or not, with evidence. Example: {"product_url":"https://owalalif…`
- `get_product`: `One listing: price per option, stock, seller, official-store flag, policy links. Example: {"product_url":"https://owalalife.com/products/fr…`
- `get_return_policy`: `Seller's return terms (window, condition, opened items, return shipping), each with the policy's exact sentence. Example: {"product_url":"h…`
- `list_brands`: `Brands with a confirmed official Shopify store, optionally by category. Example: {"category":"beauty"}`
- `search_products`: `Find products from Shopify brands; results name the seller and flag official stores. Example: {"query":"Owala FreeSip 24oz","limit":5}`

## Changes

- 2026-10-20: [annotation changed, count changed, description changed, schema changed, tool added](../../deltas/2026-10-20/bb6a0d0f9fe0ea79342b.json): `1 tool(s) added; 54 field(s) changed; signals: url_introduced`
- 2026-10-13: [count changed, tool added](../../deltas/2026-10-13/bb6a0d0f9fe0ea79342b.json): `1 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://coreplex.ai/api/apps/6a9567482e969b1ab43e0c49/functions/coreplexMcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
