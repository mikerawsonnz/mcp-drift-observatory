# agenticfabricationnetwork.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agenticfabricationnetwork.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agenticfabricationnetwork.ai/mcp` | 22 | [`41955da04970`](db3010688319f7ebe01c.json) | 2026-11-14 |

## Tools at `https://agenticfabricationnetwork.ai/mcp`

- `add_to_cart`: `Put one more part in a cart. Name it ONE way: quote_id (a quote you already have — its shops are not asked again, and the part arrives conf…`
- `check_offer`: `Run the shop's manufacturability check on ONE offer whose manufacturability_check.status is "unchecked" (the price stands from the shop's o…`
- `checkout_cart`: `Order every part of a cart with ONE payment link. Each part needs a pick that comes to exactly one option (its selection_match reads "one")…`
- `create_cart`: `Start a cart, for a user who wants several parts and one payment. Pass items to put parts in at once; each is named by quote_id (a quote yo…`
- `create_checkout`: `Create the order and get a hosted payment link for a chosen offer. Call this as soon as the user picks an offer + shipping speed. This tool…`
- `finalize_quote`: `ONLY for the case where a quote response came back with an EMPTY board and told you to call this: waits for the vendors to answer (up to ~4…`
- `fork_cart`: `Copy a cart: the same parts in the same order, each configured and picked as it was. Use it when the user opens a shared cart, so that noth…`
- `get_cart`: `Read a cart: every part with its quote, the rules on it (constraints_asked), its pick (selection) and what the pick comes to — the shop, th…`
- `get_fabrication_quote`: `Get fabrication price and delivery offers for a design file or an existing AFN part number. Supports 3D printing, CNC machining, sheet meta…`
- `get_material_guide`: `Honest, cited material intelligence for material-choice / strength / durability / heat / outdoor questions ("my PLA part broke, what's stro…`
- `get_network_capabilities`: `The LIVE catalog of what the fabrication network can do RIGHT NOW — no quote needed. Returns the services ledger (tapping, inserts, welding…`
- `get_order_status`: `Check status, ETA and tracking for a UFP order. Pass a checkout id (co_…, from checkout_cart) in order_id to get every order of that cart c…`
- `get_price_curve`: `How the per-unit price moves with quantity for a quote you already have: for every shop on the board, the item price per unit at each quant…`
- `get_shop_gauges`: `Every sheet thickness (gauge) ONE named shop stocks right now, per material — read live off the shop's declared catalog, no quote needed. C…`
- `leave_review`: `Record the user's verified-purchase review of how a UFP order turned out. YOUR JOB IS TO STRUCTURE THE FEEDBACK: turn what the user actuall…`
- `poll_quote`: `INTERNAL — the offer board calls this to refresh itself while vendors finish pricing. Never call this yourself. The board you were given is…`
- `preview_quote`: `INTERNAL client rail — the routing half of refine_quote with NOTHING committed: takes the same arguments as refine_quote and answers how ma…`
- `refine_quote`: `Narrow an existing quote with new constraints (destination ZIP the user just provided, deadline, outdoor/waterproof/heat/food-safety requir…`
- `remove_from_cart`: `Take one part out of a cart. The part's quote is untouched and can be put back with add_to_cart. Returns the whole cart. HOW A CART WORKS:…`
- `reopen_quote`: `Use when the user comes back to a part priced earlier (a saved quote_id), or when a quote carried answers_pending. A quote's answers are sh…`
- `reply_to_maker`: `Send the user's answer to a question the maker (vendor) asked about a UFP order — get_order_status surfaces an open question when one is wa…`
- `set_cart_item_quote`: `Point a part of a cart at another quote of the same part — for a part that was priced again with get_fabrication_quote. Changing a part wit…`

## Changes

- 2026-11-14: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-14/db3010688319f7ebe01c.json): `8 tool(s) added; 232 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-11-11: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-11/db3010688319f7ebe01c.json): `2 tool(s) added; 13 field(s) changed`
- 2026-11-06: [annotation changed, description changed, schema changed](../../deltas/2026-11-06/db3010688319f7ebe01c.json): `460 field(s) changed`
- 2026-11-05: [count changed, description changed, schema changed, tool removed](../../deltas/2026-11-05/db3010688319f7ebe01c.json): `1 tool(s) removed; 3 field(s) changed; signals: length_more_than_doubled`
- 2026-10-27: [description changed, schema changed](../../deltas/2026-10-27/db3010688319f7ebe01c.json): `26 field(s) changed`
- 2026-10-10: [annotation changed, field changed](../../deltas/2026-10-10/db3010688319f7ebe01c.json): `45 field(s) changed`
- 2026-09-10: [count changed, tool added](../../deltas/2026-09-10/db3010688319f7ebe01c.json): `1 tool(s) added`
- 2026-09-07: [schema changed](../../deltas/2026-09-07/db3010688319f7ebe01c.json): `17 field(s) changed; signals: length_more_than_doubled`
- 2026-09-04: [count changed, schema changed, tool added](../../deltas/2026-09-04/db3010688319f7ebe01c.json): `1 tool(s) added; 8 field(s) changed`
- 2026-09-01: [count changed, schema changed, tool added](../../deltas/2026-09-01/db3010688319f7ebe01c.json): `1 tool(s) added; 269 field(s) changed; signals: length_more_than_doubled`
- 2026-08-26: [schema changed](../../deltas/2026-08-26/db3010688319f7ebe01c.json): `2 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agenticfabricationnetwork.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
