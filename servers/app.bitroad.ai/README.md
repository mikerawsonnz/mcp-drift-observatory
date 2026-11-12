# app.bitroad.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.bitroad.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.bitroad.ai/api/v1/mcp` | 93 | [`34a31b3eb522`](e36f79dd929c8eb0f088.json) | 2026-11-12 |

## Tools at `https://app.bitroad.ai/api/v1/mcp`

- `addresses_create`: `Save a new shipping address. Set is_default_shipping=true to make it the default.`
- `addresses_list`: `List the principal's saved shipping addresses. The agent does NOT need to call this every purchase — purchase_create_intent will use the pr…`
- `auth_revoke_self`: `Disconnect this OAuth connection by revoking the access+refresh chain that issued the token making this call. Idempotent: a second call ret…`
- `auth_whoami`: `Return who this MCP credential acts as: principal email/role, agent name, client (Claude install) that issued the token, and when it was la…`
- `catalog_describe_category`: `Fetch one category by slug, including the spec JSON Schema for leaf categories. Useful before building a structured purchase intent so the…`
- `catalog_get_product`: `Fetch a single product by id. Returns full description, structured spec values, seller id, live stock, and any restricted-goods flags. Pref…`
- `catalog_list_categories`: `List the product catalog's category taxonomy. Optionally pass 'slug' to scope to a subtree (e.g. 'electronics'). Each leaf carries its JSON…`
- `catalog_search_products`: `Search the product catalog (physical goods) by free-text query, optional category, or seller. Returns a paginated list of summaries with pe…`
- `default_fund_get`: `Read the public statement of Bitroad's member loss-absorption fund: per currency (gbp, usd, eur), balance_minor, contributions_minor (net o…`
- `disputes_add_evidence`: `Attach an evidence item to an open dispute. The body is base64-encoded; per-item cap is 25 MB and per-dispute cap is 200 MB. Either the fil…`
- `disputes_file`: `File a dispute on a goods order (order_id; reasons: not_as_described, defective, not_received, fraud_unauthorized_charge, duplicate_charge,…`
- `disputes_get`: `Fetch one dispute by id with the full evidence trail and timeline. Buyer-side or seller-side caller — returns 404 if the dispute doesn't be…`
- `disputes_list`: `List disputes for the authenticated principal (buyer-side: ones they filed; seller-side: ones filed against their orders). Filter by 'statu…`
- `disputes_respond`: `Seller-side response to a dispute. Requires the seller delegation's 'respond_dispute' action. Free-form text 1–4000 chars.`
- `disputes_withdraw`: `Buyer-only: withdraw an open dispute. Closed disputes cannot be withdrawn.`
- `envelopes_get`: `Fetch a single envelope by id. Returns the same shape as envelopes_list. Returns 404 when the envelope is not bound to the calling agent in…`
- `envelopes_list`: `List the active and historical payment envelopes the calling agent instance can draw against. Each entry shows balance, scope, validity, an…`
- `factoring_quote`: `Seller side: quote what the house would pay now for one of your delivered jobs' pending credit. Returns face_pence (the credit), discount_b…`
- `factoring_sell`: `Seller side: sell one delivered job's pending credit to the house at the factoring_quote price. paid_pence is transferred to your Connect a…`
- `grades_list`: `List Bitroad's grades: the published contracts for classes of work that orders are placed against. Each active grade carries its id, slug,…`
- `index_get`: `Read Bitroad's daily price index: what each grade of work cost, per currency, for the latest published UTC day or a given date. Service ent…`
- `intents_bid`: `Seller side (respond_quote): submit or replace your sealed bid on an open intent: amount_pence (inc-VAT, at most the budget ceiling), eta_m…`
- `intents_list_open`: `Seller side (respond_quote): list open intents you can bid on, in categories where you have an active listing and in your settlement curren…`
- `intents_post`: `Post an open intent: describe the job instead of picking a listing. Give a category (optionally a capability_class such as code_review.secu…`
- `keys_claim_link`: `Key no human owns yet: get a one-hour link to hand to your principal. They open it, set an email and password, and become the owner of this…`
- `orders_book`: `Read one grade's book in one currency. A fungible grade: its token book, price levels { price_pence per million tokens, quantity_tokens, or…`
- `orders_cancel`: `Take one of your orders off the book, by the kind and id orders_list_mine returned: a listing is archived, an intent withdrawn while its bi…`
- `orders_get`: `Fetch a single order with line items, shipment / tracking, payment status, and any associated returns or disputes. Buyer-side view — for se…`
- `orders_list`: `List orders the authenticated principal placed (buyer-side view), paginated with a cursor. Optional status filter (e.g. 'paid_awaiting_fulf…`
- `orders_list_mine`: `List your resting orders on grades, newest first: a seller's asks (its active fixed-price listings on a grade, and its live token sell orde…`
- `orders_place`: `Place an order against a grade (grades_list): side 'ask' sells the grade, 'bid' buys it. A fungible grade (inference tokens) takes tokens {…`
- `panel_get_case`: `Member panel: read one case blind to the parties, with your own vote once cast. Visible to a member who may sit on it while it is open, and…`
- `panel_list_open`: `Member panel: list open dispute cases you may sit on. A case is a service dispute the acceptance engine and any verifier could not settle;…`
- `panel_vote`: `Member panel: vote release or refund on an open case, with a plain-text reason. The first 3 eligible votes count and the majority decides;…`
- `payment_methods_create`: `Returns a one-time Stripe Checkout URL to hand the user so they can add a payment card. The card is saved to their account automatically wh…`
- `payment_methods_list`: `List the principal's saved payment methods (last4 + brand only — full card numbers are never exposed to agents). purchase_confirm_intent us…`
- `platforms_get`: `Fetch a platform's public reputation profile by slug: KYC status, rolling-window orders/disputes/refunds, on-time-ship rate, dispute resolu…`
- `pricing_oracle`: `Price a job from data: for a service category (optionally one capability_class) in one currency over the last window_days (default 90), wha…`
- `procurement_memory_get`: `Buyer side: what your principal has already learned buying services on Bitroad, so a fresh agent instance does not start from zero. Your pr…`
- `purchase_cancel_intent`: `Cancel a pending purchase intent and release the stock reservation.`
- `purchase_confirm_intent`: `Confirm a purchase intent — re-validates price within 1p tolerance, charges via Stripe Connect destination charges (per-seller application…`
- `purchase_create_intent`: `Create a purchase intent for a product. Reserves stock, snapshots price + VAT + shipping, and consults the delegation policy. Returns an in…`
- `register_get`: `Fetch a store's public register entry by slug, the machine-readable record behind /stores/<slug>: identity and trust metrics, capabilities…`
- `returns_get`: `Fetch a single return by id, including reason, status, restocking fee (if any), refund ledger, and the inspection trail once the parcel has…`
- `returns_get_label`: `Fetch a short-lived signed URL for the return shipping label PDF. URL expires within minutes; re-call to get a fresh one. Only available on…`
- `returns_initiate`: `Initiate a return on a delivered order. Uniform platform policy: a 30-day change-of-mind window from delivery, FREE, full refund, NO restoc…`
- `returns_list`: `List returns the authenticated principal filed (buyer-side view), paginated. Filter by 'order_id' to find returns on a specific order, or b…`
- `seller_accept_return`: `Acknowledge that a returned parcel arrived and was inspected. Moves return: approved → received. The refund engine runs idempotently afterw…`
- `seller_archive_listing`: `Soft-delete a listing (is_active=false). Refuses while any purchase intents are still pending against it.`
- `seller_attach_tracking`: `Attach or update tracking on an already-shipped order. Use mark_shipped for first ship; this is for late-arriving tracking only.`
- `seller_create_listing`: `Create a product listing. Validates the payload against the leaf category's spec schema and the structured return policy. Restricted-goods…`
- `seller_get_listing`: `Fetch a single listing the bound seller owns, including its full description, current stock + reserved counts, spec values, and any moderat…`
- `seller_get_me`: `Fetch the seller record bound to the calling principal or seller-side agent instance. Refuses when the caller has no seller record.`
- `seller_get_order`: `Fetch a single seller-scoped order with buyer shipping address (PII-redacted where the policy requires it), items, shipment, payment status…`
- `seller_get_return`: `Fetch a single return filed against one of the bound seller's orders, with reason, status, restocking fee, inspection notes, and the refund…`
- `seller_list_listings`: `List the bound seller's product listings, paginated. Includes archived/flagged listings by default — pass 'is_active: true' to filter to li…`
- `seller_list_orders`: `List orders placed against the bound seller's products (seller-side view), paginated. Filter by 'status' (e.g. 'paid_awaiting_fulfillment'…`
- `seller_list_returns`: `List returns filed against the bound seller's orders, paginated. Filter by 'status' (initiated, label_ready, in_transit, received, refunded…`
- `seller_list_reviews`: `List reviews left on this seller's orders, paginated. Filter by 'responded: false' to find reviews that still need a seller response. A rev…`
- `seller_mark_delivered`: `Declare a shipped order as delivered (no carrier confirmation is wired). Only valid from shipped; already-delivered is a no-op success. Not…`
- and 33 more in [e36f79dd929c8eb0f088.json](e36f79dd929c8eb0f088.json)

## Changes

- 2026-11-12: [count changed, description changed, tool added](../../deltas/2026-11-12/e36f79dd929c8eb0f088.json): `2 tool(s) added; 4 field(s) changed; signals: length_more_than_doubled`
- 2026-11-10: [count changed, tool added](../../deltas/2026-11-10/e36f79dd929c8eb0f088.json): `13 tool(s) added`
- 2026-11-09: [count changed, tool added](../../deltas/2026-11-09/e36f79dd929c8eb0f088.json): `6 tool(s) added`
- 2026-11-06: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-06/e36f79dd929c8eb0f088.json): `7 tool(s) added; 21 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-10-28: [description changed, schema changed](../../deltas/2026-10-28/e36f79dd929c8eb0f088.json): `312 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.bitroad.ai/api/v1/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
