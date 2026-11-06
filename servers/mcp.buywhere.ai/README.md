# mcp.buywhere.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.buywhere.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.buywhere.ai/mcp` | 13 | [`845afb08293b`](6d3627145ce108528569.json) | 2026-09-26 |

## Tools at `https://mcp.buywhere.ai/mcp`

- `compare_products`: `Compare multiple products side-by-side. Returns price, brand, rating, and category for each.`
- `compare_products_v2`: `REQUIRED deliver_to. Compare multiple products side-by-side. Always pass deliver_to="SG" (or your buyer's country). Returns price, brand, r…`
- `find_best_price`: `Use this whenever a user asks about prices, wants to find the cheapest option, or asks "what's the best price for X" or "where can I buy X…`
- `find_best_price_v2`: `REQUIRED deliver_to. Use this whenever a user asks about prices, wants to find the cheapest option, or asks "what's the best price for X" o…`
- `find_similar`: `Find products similar to a given product using vector similarity. Returns up to 10 nearest neighbours by semantic meaning (title+descriptio…`
- `get_deals`: `Get discounted products sorted by discount percentage. Returns schema.org/Product entities with schema.org/Offer properties: price, priceCu…`
- `get_deals_v2`: `REQUIRED deliver_to. Get discounted products sorted by discount percentage. Always pass deliver_to="SG" (or your buyer's country). Returns…`
- `get_product`: `Get a specific product by its ID, including full details and current price.`
- `get_product_v2`: `REQUIRED deliver_to. Get a specific product by its ID, including full details and current price. Always pass deliver_to="SG" (or your buyer…`
- `ingest_products`: `Ingest (upsert) a batch of products into the BuyWhere catalog. Use this to add or update product listings from any merchant/source. Require…`
- `list_categories`: `List top-level product categories available in the BuyWhere catalog.`
- `search_products`: `Search the BuyWhere product catalog by keyword. Treat deliver_to as REQUIRED for buyer-facing use (ISO-3166 country of the end user); it ta…`
- `search_products_v2`: `REQUIRED deliver_to. Search the BuyWhere product catalog by keyword. The deliver_to parameter is REQUIRED (ISO country code, e.g. "SG", "US…`

## Changes

- 2026-09-26: [description changed, schema changed](../../deltas/2026-09-26/6d3627145ce108528569.json): `6 field(s) changed`
- 2026-09-18: [schema changed](../../deltas/2026-09-18/6d3627145ce108528569.json): `4 field(s) changed`
- 2026-09-15: [schema changed](../../deltas/2026-09-15/6d3627145ce108528569.json): `4 field(s) changed`
- 2026-09-03: [description changed](../../deltas/2026-09-03/6d3627145ce108528569.json): `3 field(s) changed`
- 2026-09-02: [description changed, schema changed](../../deltas/2026-09-02/6d3627145ce108528569.json): `6 field(s) changed`
- 2026-08-31: [description changed, schema changed](../../deltas/2026-08-31/6d3627145ce108528569.json): `25 field(s) changed`
- 2026-08-27: [count changed, description changed, schema changed, tool added](../../deltas/2026-08-27/6d3627145ce108528569.json): `5 tool(s) added; 13 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled, url_introduced` **(notable)**
- 2026-08-26: [count changed, schema changed, tool removed](../../deltas/2026-08-26/6d3627145ce108528569.json): `5 tool(s) removed; 8 field(s) changed`
- 2026-08-24: [description changed, schema changed](../../deltas/2026-08-24/6d3627145ce108528569.json): `19 field(s) changed`
- 2026-08-22: [count changed, description changed, schema changed, tool added](../../deltas/2026-08-22/6d3627145ce108528569.json): `5 tool(s) added; 39 field(s) changed; signals: url_introduced`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.buywhere.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
