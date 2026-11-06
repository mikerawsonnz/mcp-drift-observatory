# marketcrew.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/marketcrew.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://marketcrew.ai/mcp` | 15 | [`3327585d7c66`](282bd5514238b95c0739.json) | 2026-08-20 |

## Tools at `https://marketcrew.ai/mcp`

- `get_crypto_context`: `Crypto market context for a technical read: BTC/ETH dominance and total/alt market cap, Fear & Greed sentiment, perp funding rate & open in…`
- `get_event_stats`: `Historical base rates for the technical events firing on a ticker today (e.g. RSI below 30, golden/death cross, new 52-week high/low). For…`
- `get_instrument_info`: `Get current information about a financial instrument: price, price changes, market state, 52-week range, earnings date. Provide either inst…`
- `get_intermarket`: `Intermarket compass — a first-pass read of the market environment through price-ratio lenses: asset-class rotation (bonds vs stocks, commod…`
- `get_key_levels`: `Compute key price levels for a ticker: support/resistance zones (clustered swing highs/lows with touch counts = how often price reacted the…`
- `get_macro_context`: `Get macro market context: sector P/E ratios, sector performance, US Treasury rates (2Y/10Y/30Y), CPI inflation data. Also provides key inte…`
- `get_market_breadth`: `S&P 500 market breadth: the percentage of index members above their 50-day and 200-day moving averages, with RSI, trend and 52-week range f…`
- `get_monitoring_options`: `Returns available options for ongoing monitoring — price alerts, idea tracking, watchlist monitoring, scheduled digests — with setup instru…`
- `get_price_history`: `Get daily OHLCV price history for a ticker: open/high/low/close/volume. Use period_days to control how far back (default 365, max 3650).`
- `get_relative_strength`: `Calculate relative strength ratio between two tickers (A/B). Returns current ratio, SMA(50)/SMA(200) of ratio, RSI of ratio, trend directio…`
- `get_sentiment_data`: `Get market sentiment indicators: CBOE Put/Call ratios (total, equity, index, VIX), AAII investor sentiment survey (bull/bear/neutral %), an…`
- `get_ta_methodology`: `Look up MarketCrew's distilled technical-analysis methodology — our own synthesized notes on how to read indicators, structure, levels and…`
- `get_technical_indicators`: `Calculate technical indicators for a ticker: SMA(50/200), RSI(14), MACD, ATR(14), ADX(14) trend strength, Stochastic(14,3), volume (OBV tre…`
- `public_instrument_news`: `Latest news for a ticker — headline, a short summary and a mandatory source_url to the original article (never the full third-party text).…`
- `public_search_news`: `Semantic news search across tracked instruments — returns matching items with a short summary and a mandatory source_url (never full articl…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://marketcrew.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
