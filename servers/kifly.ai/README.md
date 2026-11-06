# kifly.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/kifly.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://kifly.ai/api/mcp` | 21 | [`d70d6098767b`](26b4ae2416864b7bf6ec.json) | 2026-08-22 |

## Tools at `https://kifly.ai/api/mcp`

- `add_to_cart`: `Requires 'checkout:write' scope. Add a product variant to an existing cart. Use the variant_id from search_products results. Returns full c…`
- `checkout`: `Requires 'checkout:write' scope. **Requires 'set_shipping_address' to have been called first.** Returns 400 'invalid_shipping' if no addres…`
- `create_cart`: `Create a new shopping cart on Kifly. **For network (cross-seller) tokens you MUST pass 'seller_handle'** — each cart is bound to exactly on…`
- `get_buyer_profile`: `Retrieve a repeat buyer's saved name, email, and default shipping address. **At the start of every purchase flow, ask the buyer in plain la…`
- `get_cart`: `Inspect the current state of a cart — line items, quantities, prices, and shipping address. Each item includes an 'item_id' you can pass to…`
- `get_help`: `Get Kifly's website and support contact email. Call this if you are stuck, hit an unresolvable error, or the buyer asks how to reach a huma…`
- `get_platform_limits`: `Returns the current platform-enforced cart limits: 'max_item_quantity' (per-line-item ceiling), 'max_cart_total_cents', and 'max_cart_total…`
- `get_seller`: `Retrieve a seller's public profile: name, location (city/region/country), storefront URL, delivery fee, delivery coverage, and catalog size…`
- `list_orders`: `List a returning buyer's recent orders and their current fulfillment status — use this in a NEW session to answer 'did my order ship?' / 'w…`
- `list_sellers`: `List all active sellers on the Kifly network. **Requires a network token (kfn_live_…).** Returns each seller's handle, name, city, region,…`
- `order_status`: `Check the status of a Stripe checkout session. Poll every 5 seconds after checkout until status is 'paid', 'shipped', or 'failed'. Returns…`
- `quick_buy`: `Requires 'cart:write' scope. Create a cart, add items, and set the shipping address in ONE call — the fast path when you already know the s…`
- `register_buyer`: `Start registering a buyer so they can be recognized across future purchases without re-entering their details. Takes the buyer's email and…`
- `request_buyer_code`: `Send a 6-digit verification code to a **returning** buyer's email so they can prove the account is theirs and recover their saved name + sh…`
- `request_feature`: `Submit the buyer's **product/feature request** to the Kifly team. Use this when the buyer wishes Kifly *itself* did something it doesn't —…`
- `save_buyer_address`: `Save a shipping address to the buyer's Kifly profile so it auto-fills on future purchases. **Call this after a successful checkout if 'get_…`
- `search_products`: `Search or browse Kifly's product catalog. Multilingual semantic search (100+ languages). Returns a JSON-LD ItemList with 'kifly:totalCatalo…`
- `set_shipping_address`: `Requires 'checkout:write' scope. Persist a shipping address on the cart and confirm whether the seller can deliver to it. **Call BEFORE 'ch…`
- `submit_feedback`: `Send structured feedback to the Kifly team. **Call after a confusing response, a dead-end, or a successful workaround you had to invent** —…`
- `update_cart_item`: `Requires 'checkout:write' scope. Change the quantity of a line item in an open cart, or remove it entirely. Set 'quantity' to 0 to remove t…`
- `verify_buyer`: `Verify the 6-digit code a returning buyer received by email (from 'request_buyer_code'). On success returns '{ buyer_token, buyer_profile_i…`

## Changes

- 2026-08-22: [description changed](../../deltas/2026-08-22/26b4ae2416864b7bf6ec.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://kifly.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
