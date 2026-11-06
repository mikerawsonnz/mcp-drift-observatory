# genosys.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/genosys.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://genosys.ae/mcp` | 11 | [`9248b9bafac7`](888eb89ee5853bde30c3.json) | 2026-10-13 |

## Tools at `https://genosys.ae/mcp`

- `create_bag_link`: `Build one link that opens genosys.ae with these items already in the shopper's bag, ready to check out. Use when the shopper decides to buy…`
- `fetch`: `Full text of a result from search, by id ("product:18" or "blog:<slug>").`
- `get_product`: `Full details for one product: description, key features, benefits, key ingredients and actives, step-by-step how to use, sizes or shades wi…`
- `list_categories`: `All product categories and skin concerns in the live catalog, with product counts. Use to orient before searching.`
- `open_checkout`: `Show the shopper a checkout form for these items: shade picker where needed, quantities, delivery details (name, email, phone, emirate, add…`
- `order_status`: `Status and payment of a GENOSYS order. Needs the order number and the email used for the order.`
- `place_order`: `Create a GENOSYS UAE order from this chat and get a secure Stripe payment link (card, Apple Pay, Google Pay). Call only after the shopper h…`
- `recommend_routine`: `Ranked product picks for a shopper's skin type and concerns, the same scoring as the skin quiz on genosys.ae. Use when someone describes th…`
- `search`: `Search GENOSYS products and skincare articles. Returns ids to pass to fetch. ("product:<id>" for products, "blog:<slug>" for articles.)`
- `search_products`: `Search the live GENOSYS UAE catalog (Korean professional skincare, haircare, devices, beauty boxes). Use for any "what do you have for..."…`
- `store_info`: `Delivery areas, times and fees, payment methods, returns, contact (WhatsApp, email), apps and policies for GENOSYS UAE.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://genosys.ae/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
