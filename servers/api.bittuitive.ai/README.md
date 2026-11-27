# api.bittuitive.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.bittuitive.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.bittuitive.ai/mcp` | 41 | [`cd5fef5a108c`](c0c8c3bdf1cbda3c2fcd.json) | 2026-11-27 |

## Tools at `https://api.bittuitive.ai/mcp`

- `ack_feed_mailbox_item`: `Use this when marking a mailbox item handled so it hides from default get_feed_mailbox results. Safe to repeat.`
- `browse_scoreboard`: `Use this when surveying paid agent APIs by 0-100 score (view="search") or per-category stats (view="categories"). Free, read-only.`
- `buy_credits`: `Use this when prepaying a btf_ balance (starter 1,000 sats/$1, standard 5,000/$5, bulk 25,000/$25; 365-day expiry; redeemable only for BitT…`
- `call_routed_api`: `Use this when calling a third-party L402 API or capability (ai_inference with prompt/messages from ~$0.0024; web_search with query) with on…`
- `check_domain`: `Use this when checking DNS, RDAP registration, TLS, email MX/disposable, phone format/region, or IP/ASN before contacting/paying/signing up…`
- `contribute_bittuition`: `Use this when submitting a BitTuition sentiment vote (0-100 or bullish/neutral/bearish) on an allowlisted stock, crypto, or AI subject (no…`
- `convert_pdf`: `Use this when extracting clean Markdown/text from a PDF (self-hosted). Pass url or file_base64 and optional pages (max 20 MB, 100 pages; te…`
- `create_feed`: `Use this when avoiding polling: push data on a schedule or trigger to webhook_url and/or 72h mailbox. Creating is free; deliveries debit pr…`
- `delete_feed`: `Use this when removing a feed. PERMANENTLY deletes the feed definition and stops future deliveries (cannot be undone; prefer update_feed st…`
- `fetch_page`: `Use this to read a public web page as Markdown (URL to Markdown, self-hosted, no JS; use convert_pdf for PDFs). Pass url. Price: $0.002 fla…`
- `find_best_endpoint`: `Use this when you need a paid data API by keyword (e.g. 'bitcoin price', 'air quality', 'stock fundamentals') ranked by 0-100 quality score…`
- `get_ai_buildout`: `Use this when you need the AI Buildout headline from SEC filings (company-wide capex, YoY growth, acceleration) for optional symbol (e.g. M…`
- `get_ai_data`: `Use this when a research agent needs AI Buildout trends from SEC filings (company-wide capex, revenue, cash flow; optional symbol, else uni…`
- `get_alerts_data`: `Use this when an agent needs US government alerts (USGS earthquakes, CISA KEV, openFDA recalls, Federal Register). Pass stream (default usg…`
- `get_bitcoin_price`: `Use this when you need the current Bitcoin price (BTC/USD, btc price). Returns btc_intuitive multi-source price + Data BitScore. Price: 5 s…`
- `get_bittuition`: `Use this when an agent needs BitTuition sentiment (0-100: 100=bullish, 50=neutral, 0=bearish) on allowlisted stocks, cryptos, or AI subject…`
- `get_btc_data`: `Use this when an agent needs Bitcoin data (BTC/USD, btc price, fees, mempool, sentiment). kind="intuitive" (default; also get_bitcoin_price…`
- `get_company_data`: `Use this when an agent needs a company lookup for KYB/business verification: legal name, status, jurisdiction, address, LEI/CIK/ticker, mat…`
- `get_credit_balance`: `Use this when checking remaining prepaid sats and USDC balance for credit_token. Read-only.`
- `get_crypto_prices`: `Use this when you need BTC and/or ETH USD prices in one short call. Pass symbols (default "BTC,ETH"). Price: 3 sats or $0.002 USDC. Pay: L4…`
- `get_expense_data`: `Use this when you need expense data. Returns JSON 'data' with attribution. Kinds: intuitive (5 sats or $0.003 USDC: Use this when an agent…`
- `get_feed_mailbox`: `Use this when reading stored feed deliveries (kept 72h; unacked by default, or item_id / include_acked=true). Read-only.`
- `get_feeds`: `Use this when checking your feeds and prepaid balance (or one feed's status/schedule via feed_id). Read-only.`
- `get_finance_data`: `Use this when an agent needs official daily FX reference rates (ECB, Bank of Canada) with Data BitScore. kind="intuitive" (default): one pa…`
- `get_insights_data`: `Use this when deciding what data to build or price from k-anonymized agent demand. kind="intuitive": headline; kind="stats": willingness to…`
- `get_market_insights`: `Use this when you want a build-next signal from k-anonymized agent demand (supply-demand gaps, 30-day funnel). Same as get_insights_data(ki…`
- `get_pricing`: `Use this when checking current per-call sats/USDC prices, credit bundles, and subscription plans. Free, read-only.`
- `get_rates_data`: `Use this when an agent needs Fed, ECB, and Bank of Canada policy rates and US Treasury yield curve. kind="intuitive" (default): policy rate…`
- `get_scoreboard_entry`: `Use this when checking due diligence (score breakdown, uptime, latency, probe history) for a scoreboard id. Free, read-only.`
- `get_seller_data`: `Use this when an agent is about to pay a seller and needs a counterparty, price-fairness, and uptime screen. kind="intuitive" (default): ve…`
- `get_stock_data`: `Use this when an agent needs legacy SEC fundamentals or filings (prefer get_stocks_data). Pass symbol (default AAPL). Returns JSON 'data' w…`
- `get_stocks_data`: `Use this when an agent needs computed SEC EDGAR financials and parsed Form 4 insider trades. Pass symbol (default AAPL). kind="intuitive" (…`
- `get_travel_data`: `Use this when an agent needs US airport delays, ground stops, or closures. kind="intuitive" (default; optional airport, default SFO): brief…`
- `get_trust_data`: `Use this when an agent must screen a person, entity, or crypto/Lightning/x402 payee against US OFAC and UK sanctions or check counterparty…`
- `get_weather`: `Use this when an agent needs weather with Data BitScore. kind="intuitive" (default): current conditions; kind="stats": 7-day forecast; kind…`
- `list_routable_apis`: `Use this when listing scoreboard-verified L402 APIs the router can call with upstream price, fee, and total sats. Free, read-only. Next: ca…`
- `list_route_capabilities`: `Use this when checking capabilities BitTuitive can route (ai_inference, web_search, etc.), preferences, and approved source counts. Free, r…`
- `request_endpoint`: `Use this when no tool has the data you need: describe it and we log demand; similar requests merge into votes. Pass id to upvote an existin…`
- `run_ai_inference`: `Use this when you need an open-weight LLM completion with no API key. Pass prompt or messages, optional model and max_tokens (default 1024,…`
- `search_web`: `Use this for live web search (title, URL, snippet, source, date). Pass query. Price: about $0.007 (upstream + fee max(20%, 3 sats)). Same a…`
- `update_feed`: `Use this when changing a feed's interval, trigger, params, webhook_url, mailbox, or state (paused/active). Free; safe to repeat.`

## Changes

- 2026-11-27: [description changed, tool added, tool removed](../../deltas/2026-11-27/c0c8c3bdf1cbda3c2fcd.json): `1 tool(s) added; 1 tool(s) removed; 2 field(s) changed`
- 2026-11-26: [count changed, description changed, field changed, schema changed, tool added, tool removed](../../deltas/2026-11-26/c0c8c3bdf1cbda3c2fcd.json): `6 tool(s) added; 4 tool(s) removed; 438 field(s) changed; signals: length_more_than_doubled, url_introduced`
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
