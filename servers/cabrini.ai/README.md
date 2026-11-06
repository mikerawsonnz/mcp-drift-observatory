# cabrini.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/cabrini.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://cabrini.ai/mcp` | 15 | [`daff1e6176e0`](de7288882ccd07d524fd.json) | 2026-08-20 |

## Tools at `https://cabrini.ai/mcp`

- `get_bars`: `Resampled intraday bars at custom timeframes (3, 6, 9, 12, 15, 30, 60, 240 min) for one ticker. Every bar carries absolute open/high/low/cl…`
- `get_brief`: `Full research brief: price, fundamentals, insiders, splits for one ticker. $0.25 USDC.`
- `get_company`: `Company profile: name, CIK, industry, exchange, fiscal year. $0.005 USDC.`
- `get_filings`: `SEC filing index (10-K, 10-Q, 8-K, proxies) for a ticker. $0.01 USDC; add sections=[risk_factors, mdna] to extract full section text from t…`
- `get_fundamentals`: `Quarterly fundamentals from SEC EDGAR (revenue, EPS, margins, etc). $0.02 USDC.`
- `get_insiders`: `Insider transactions (Form 4) from SEC EDGAR. $0.02 USDC.`
- `get_pricing`: `Pricing and data coverage information. Free.`
- `get_sample`: `FREE, no payment: real intraday OHLCV bars for AAPL on 2024-01-02, identical in shape to a paid query. Call this first to verify data quali…`
- `get_stats`: `Platform statistics. Free.`
- `list_tickers`: `List all tickers that traded on a given date. $0.005 USDC.`
- `query_batch`: `Multiple tickers for one date. Every bar carries absolute open/high/low/close plus fractional change from that ticker's own daily open. $0.…`
- `query_daily`: `Daily OHLCV bars plus VWAP, range_pct and true_range_pct for one ticker over a date range. range_pct = (high - low) / open is a ready-made…`
- `query_minute_bars`: `Full trading day of intraday bars for one US stock (interval 3-240 min, default 3m). Every bar carries absolute open/high/low/close plus pc…`
- `query_range`: `Multi-day intraday bars for one ticker (interval 3-240 min, default 3m). Every bar carries absolute open/high/low/close plus fractional cha…`
- `scan_market`: `Scan all US stocks on a date for custom criteria (gaps, volume, change). Returns pct_change, range_pct, pct_gap, true_range_pct, volume and…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://cabrini.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
