# api.bittuitive.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.bittuitive.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.bittuitive.ai/mcp` | 39 | [`62c2624a82dc`](c0c8c3bdf1cbda3c2fcd.json) | 2026-11-25 |

## Tools at `https://api.bittuitive.ai/mcp`

- `ack_feed_mailbox_item`: `Use this when you have processed a mailbox item, so it stops appearing in the default list. Does not delete it (it still expires after 72 h…`
- `browse_scoreboard`: `Use this when you want to survey the market instead of getting one pick: list paid agent APIs by score with filters (view="search": q, data…`
- `buy_credits`: `Use this when you will make many calls or run feeds and want to pay once instead of per call. Suggested bundles: starter 1,000 sats / $1, s…`
- `call_routed_api`: `Use this when you want data from another paid API without handling its invoice: pay ONE BitTuitive invoice (sats, or the same all-in price…`
- `check_domain`: `Use this when you need DNS, registration, TLS, email, phone or IP facts about a contact. Self-hosted on BitTuitive hardware (no upstream).…`
- `contribute_bittone`: `Use this when your agent wants to contribute a structured 0-100 score to BitTone (50 is neutral). Tickers, coins, AI models and AI topics a…`
- `convert_pdf`: `Use this when you need clean Markdown or plain text from a PDF. Self-hosted on BitTuitive hardware (no upstream). Pass url (a public http(s…`
- `create_feed`: `Use this when an agent would otherwise poll: get data pushed on a schedule (e.g. hourly BTC price) or when a trigger fires (BTC moves 2%, p…`
- `delete_feed`: `Use this when you no longer want a feed. PERMANENTLY deletes the feed definition and stops all future deliveries; this cannot be undone (cr…`
- `fetch_page`: `Use this when you need the readable text of a public web page as clean Markdown. Self-hosted on BitTuitive hardware (no upstream). Pass url…`
- `find_best_endpoint`: `Use this when your task needs a paid data API you have not picked yet (e.g. 'bitcoin price', 'btc price', 'air quality', 'stock fundamental…`
- `get_ai_buildout`: `Use this when a research agent needs a quick headline for one company or the whole AI buildout: capex, year-over-year growth and whether it…`
- `get_ai_data`: `Use this when a research agent needs AI Buildout trends from company regulatory filings (company-wide capex, revenue and cash flow, not an…`
- `get_airport_data`: `Use this when a travel agent needs US airport status: one-airport briefing (kind="intuitive", the default; pass airport=SFO or omit to defa…`
- `get_alerts_data`: `Use this when an agent needs official US government alert streams: USGS earthquakes, CISA Known Exploited Vulnerabilities, openFDA drug rec…`
- `get_bitcoin_price`: `Use this when you need the current Bitcoin price (BTC/USD, btc price). Returns BitTuitive's recommended btc_intuitive value: a price checke…`
- `get_bittone`: `Use this when an agent needs BitTone, the first-party consensus of agent-submitted scores on an allowlisted stock, crypto, or AI subject. T…`
- `get_btc_data`: `Use this when an agent needs Bitcoin data. For the current Bitcoin price (BTC/USD, btc price), start with kind="intuitive" (the default; al…`
- `get_credit_balance`: `Use this when you want to know how much prepaid balance (sats and USDC) is left before running more calls or feeds. Read-only. Example: get…`
- `get_expense_data`: `Use this when you need expense data. Returns JSON in the 'data' field with source attribution. Read-only; the only side effect is the payme…`
- `get_feed_mailbox`: `Use this when you want the deliveries stored for you (a feed without a webhook, or one whose webhook failed): lists unacknowledged items, o…`
- `get_feeds`: `Use this when you need to check your feeds: without feed_id it lists every feed and the prepaid sats balance; with feed_id it returns that…`
- `get_finance_data`: `Use this when an agent needs official daily FX reference rates (ECB and Bank of Canada), with a Data BitScore. kind="intuitive" (the defaul…`
- `get_insights_data`: `Use this when you are deciding what data to build, source or price, or want to know what other AI agents ask for and pay for. kind="intuiti…`
- `get_market_insights`: `Use this when you want a derived build-next signal from agent demand: supply-demand gaps and the 30-day payment conversion funnel. Aggregat…`
- `get_pricing`: `Use this when you need current prices before spending: per-call sats and USDC for every BitTuitive data endpoint, credit bundles, subscript…`
- `get_rates_data`: `Use this when an agent needs official Fed, ECB and Bank of Canada policy rates and the official Treasury par yield curve. kind="intuitive"…`
- `get_sanctions_data`: `Use this when an agent is about to pay, transfer, trade or onboard and must check whether a person, entity or crypto address appears on US…`
- `get_scoreboard_entry`: `Use this when you need due diligence before you pay or route: given an id from find_best_endpoint or browse_scoreboard, returns the score c…`
- `get_seller_data`: `Use this when an agent is about to pay a seller and needs a screening aid that bundles the trust_signals counterparty check, price fairness…`
- `get_stock_data`: `Use this when a research agent needs the legacy SEC fundamentals snapshot (kind="fundamentals") or the stock_filings alias (kind="filings",…`
- `get_stocks_data`: `Use this when a research agent needs computed SEC fundamentals and parsed Form 4 insider trades, not raw reprints: the latest-quarter snaps…`
- `get_travel_data`: `Use this when a travel agent needs US airport status: one-airport briefing (kind="intuitive", the default; pass airport=SFO or omit to defa…`
- `get_trust_data`: `Use this when an agent is about to pay, transfer, trade or onboard and must check whether a person, entity or crypto address appears on US…`
- `get_weather`: `Use this when an agent needs weather, Data BitScored: current conditions (kind="intuitive", the default), a 7-day forecast (kind="stats"),…`
- `list_routable_apis`: `Use this when you need data BitTuitive does not sell directly and want it paid for you: lists every scoreboard-verified L402 API the router…`
- `list_route_capabilities`: `Use this when you need a data point BitTuitive does not sell as one of Ours (direct) endpoints: lists capabilities, available preferences (…`
- `request_data`: `Use this when no tool covers the data you need (e.g. air quality, crypto OHLC, flight prices): records one demand signal (data_type, descri…`
- `update_feed`: `Use this when you want to change a feed: interval, trigger, params, webhook_url, mailbox, or pause/resume it with 'state'. Only the fields…`

## Changes

- 2026-11-25: [count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-25/c0c8c3bdf1cbda3c2fcd.json): `3 tool(s) added; 22 field(s) changed; signals: url_introduced`
- 2026-11-24: [count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-24/c0c8c3bdf1cbda3c2fcd.json): `6 tool(s) added; 78 field(s) changed; signals: length_more_than_doubled, url_introduced`
- 2026-11-23: [count changed, description changed, schema changed, tool added, tool removed](../../deltas/2026-11-23/c0c8c3bdf1cbda3c2fcd.json): `3 tool(s) added; 1 tool(s) removed; 78 field(s) changed; signals: url_introduced`
- 2026-11-22: [count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-22/c0c8c3bdf1cbda3c2fcd.json): `7 tool(s) added; 29 field(s) changed; signals: length_more_than_doubled, url_introduced`
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
