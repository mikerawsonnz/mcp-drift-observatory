# api.bittuitive.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.bittuitive.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.bittuitive.ai/mcp` | 21 | [`007bae66d206`](c0c8c3bdf1cbda3c2fcd.json) | 2026-11-21 |

## Tools at `https://api.bittuitive.ai/mcp`

- `ack_feed_mailbox_item`: `Use this when you have processed a mailbox item, so it stops appearing in the default list. Does not delete it (it still expires after 72 h…`
- `browse_scoreboard`: `Use this when you want to survey the market instead of getting one pick: list paid agent APIs by score with filters (view="search": q, data…`
- `buy_credits`: `Use this when you will make many calls or run feeds and want to pay once instead of per call. Omit credit_token to open a new account: the…`
- `call_routed_api`: `Use this when you want data from another paid API without handling its invoice: pay ONE BitTuitive invoice (sats, or the same all-in price…`
- `create_feed`: `Use this when an agent would otherwise poll: get data pushed on a schedule (e.g. hourly BTC price) or when a trigger fires (BTC moves 2%, p…`
- `delete_feed`: `Use this when you no longer want a feed. PERMANENTLY deletes the feed definition and stops all future deliveries; this cannot be undone (cr…`
- `find_best_endpoint`: `Use this when your task needs a paid data API you have not picked yet (e.g. 'bitcoin price', 'air quality', 'stock fundamentals') and you w…`
- `get_airport_data`: `Use this when a travel agent must know whether a US airport has delays, a ground stop or a closure before booking, rebooking or telling a u…`
- `get_btc_data`: `Use this when an agent needs Bitcoin data: the current BTC price (trading and treasury bots, pricing an invoice in USD, spotting a >2% move…`
- `get_credit_balance`: `Use this when you want to know how much prepaid balance (sats and USDC) is left before running more calls or feeds. Read-only. Example: get…`
- `get_feed_mailbox`: `Use this when you want the deliveries stored for you (a feed without a webhook, or one whose webhook failed): lists unacknowledged items, o…`
- `get_feeds`: `Use this when you need to check your feeds: without feed_id it lists every feed and the prepaid sats balance; with feed_id it returns that…`
- `get_fx_data`: `Use this when an agent needs official daily foreign-exchange reference rates for USD, EUR, CAD and common crosses, with a Data BitScore fro…`
- `get_market_insights`: `Use this when you are deciding what data to build, source or price, or want to know what other AI agents ask for and pay for: ranked reques…`
- `get_pricing`: `Use this when you need current prices before spending: per-call sats and USDC for every BitTuitive data endpoint, credit bundles, subscript…`
- `get_scoreboard_entry`: `Use this when you need due diligence before you pay or route: given an id from find_best_endpoint or browse_scoreboard, returns the score c…`
- `get_stock_data`: `Use this when a research agent needs US company financials or SEC filings for a ticker (SEC EDGAR): revenue, EPS and debt, or the latest 10…`
- `get_weather`: `Use this when an agent needs weather (NOAA NWS and MET Norway, Data BitScored): current conditions, a 7-day forecast or severe-weather aler…`
- `list_routable_apis`: `Use this when you need data BitTuitive does not sell directly and want it paid for you: lists every scoreboard-verified L402 API the router…`
- `request_data`: `Use this when no tool covers the data you need (e.g. air quality, crypto OHLC, flight prices): records one demand signal (data_type, descri…`
- `update_feed`: `Use this when you want to change a feed: interval, trigger, params, webhook_url, mailbox, or pause/resume it with 'state'. Only the fields…`

## Changes

- 2026-11-21: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-21/c0c8c3bdf1cbda3c2fcd.json): `1 tool(s) added; 9 field(s) changed`
- 2026-11-20: [annotation changed, count changed, description changed, field changed, schema changed, tool added, tool removed](../../deltas/2026-11-20/c0c8c3bdf1cbda3c2fcd.json): `15 tool(s) added; 29 tool(s) removed; 56 field(s) changed; signals: credential_shaped_string_introduced, imperative_language_introduced, le…` **(notable)**
- 2026-11-19: [count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-19/c0c8c3bdf1cbda3c2fcd.json): `2 tool(s) added; 31 field(s) changed; signals: length_more_than_doubled`
- 2026-11-18: [description changed, field changed, schema changed](../../deltas/2026-11-18/c0c8c3bdf1cbda3c2fcd.json): `4 field(s) changed`
- 2026-11-17: [count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-17/c0c8c3bdf1cbda3c2fcd.json): `12 tool(s) added; 49 field(s) changed; signals: imperative_language_introduced, url_introduced` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.bittuitive.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
