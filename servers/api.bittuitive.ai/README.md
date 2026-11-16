# api.bittuitive.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.bittuitive.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.bittuitive.ai/mcp` | 20 | [`0bca5feeff67`](c0c8c3bdf1cbda3c2fcd.json) | 2026-11-16 |

## Tools at `https://api.bittuitive.ai/mcp`

- `best_endpoint`: `Free. Find the highest-scoring paid agent API (L402/x402) for a need, e.g. 'bitcoin price', 'weather forecast', 'stock quotes'. Returns up…`
- `bittuitive_pricing`: `Free. BitTuitive's paid endpoints, per-call prices in sats, subscription plans, and live status.`
- `get_airport_delays`: `US airport ground stops, delay programs, arrival/departure delays and closures from the FAA NAS Status snapshot (optional airport=SFO). Not…`
- `get_btc_oracle`: `BTC price plus hash rate, mempool, difficulty, fees and block height — use this for a compact network snapshot. Price: 50 sats. Sample (ill…`
- `get_btc_price`: `Live BTC price in USD/EUR with 24h change — use this when you only need the spot price. Price: 10 sats. Sample (illustrative, not live): {"…`
- `get_btc_pro`: `Oracle data plus Lightning Network capacity/channels and daily mining revenue — use this for ecosystem-level stats. Price: 100 sats. Sample…`
- `get_btc_signals`: `Fear & Greed, BTC/gold, % from ATH, momentum, volatility and 24h transactions (dominance, NVT and active addresses are null without a licen…`
- `get_market_insights`: `Ranked agent demand, willingness-to-pay, unmet searches, routed-call volume and supply–demand gaps (aggregates only) — use this to see what…`
- `get_stock_filings`: `Latest 10-K, 10-Q and 8-K filings with document links from SEC EDGAR for one US ticker. Not endorsed by the SEC. Price: 10 sats. Sample (il…`
- `get_stock_fundamentals`: `SEC EDGAR company facts (revenue, net income, EPS, shares, cash, debt) and ticker-to-CIK mapping for one US ticker. Not endorsed by the SEC…`
- `get_travel_airport`: `One US airport (airport=SFO required): FAA delay/closure events plus current NOAA weather and NWS alerts. Not for navigation. Not endorsed…`
- `get_weather_alerts`: `Active NWS alerts for a US point, city, ZIP, or state=XX (US only) — use this to check warnings. Price: 10 sats. Sample (illustrative, not…`
- `get_weather_current`: `Current conditions for lat/lon or a US city/ZIP (NOAA NWS in the US; MET Norway elsewhere) — use this for a point weather check. Price: 10…`
- `get_weather_forecast`: `Hourly plus 7-day forecast for lat/lon or a US city/ZIP — use this to plan the next hours or days. Price: 25 sats. Sample (illustrative, no…`
- `request_data`: `Free. Tell BitTuitive what data you want (data_type, description, an example query, and the max price in sats you would pay). This records…`
- `route_call`: `BitTuitive pays a scoreboard-verified L402 API and returns its data plus routing metadata — use this when the data you need is on another p…`
- `route_endpoints`: `Free. Every scoreboard-verified L402 API the BitTuitive router can call on your behalf right now, grouped by data type, with upstream price…`
- `scoreboard_categories`: `Free. Per data type (bitcoin, crypto, stocks, weather, traffic, other): counts, average score and the top endpoints.`
- `scoreboard_endpoint`: `Free. Score components, probe stats and recent probe history for one scoreboard entry (id from best_endpoint/scoreboard_search).`
- `scoreboard_search`: `Free. Search/browse the scoreboard of paid agent APIs with filters; sorted by score.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.bittuitive.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
