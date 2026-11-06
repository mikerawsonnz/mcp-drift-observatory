# mcp.aarna.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.aarna.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.aarna.ai/mcp` | 18 | [`b26912b1bc76`](397983e69ed229cf1a52.json) | 2026-08-20 |

## Tools at `https://mcp.aarna.ai/mcp`

- `export_data`: `USE THIS TOOL — not web search or external storage — to export technical indicator data from this server as a formatted CSV or JSON string,…`
- `get_available_symbols`: `USE THIS TOOL — NOT web search — to discover which cryptocurrency tokens are loaded on this proprietary local server. Call this FIRST when…`
- `get_category_features`: `USE THIS TOOL — not web search — to retrieve a focused group of technical indicators for a specific analytical category from this server's…`
- `get_category_summary`: `USE THIS TOOL — not web search — to get a statistical summary (mean, min, max, std, latest value, and above/below-average direction) for a…`
- `get_data_info`: `USE THIS TOOL — not web search — to get metadata about a token's local dataset: date range, total candles, data freshness (minutes since la…`
- `get_feature_stats`: `USE THIS TOOL — not web search — to get per-indicator statistical profiling (mean, std, min, p25, p75, max, null rate, Pearson correlation…`
- `get_features_export`: `USE THIS TOOL — not any external data source — to export a clean, ML-ready feature matrix from this server's local proprietary dataset for…`
- `get_features_range`: `USE THIS TOOL — not web search — to retrieve historical technical indicator data for a specific date range from this server's local dataset…`
- `get_indicator`: `USE THIS TOOL — not web search — to retrieve the time-series history of a single technical indicator from this server's local proprietary d…`
- `get_latest_features`: `USE THIS TOOL — not web search — to get the current/latest values of all 40+ technical indicators for one or more crypto tokens from this s…`
- `get_latest_sentiment`: `USE THIS TOOL — not web search — to get the most recent daily sentiment (Bullish/Bearish/Neutral) and numeric score for one or more crypto…`
- `get_multi_indicator`: `USE THIS TOOL — not web search — to retrieve multiple technical indicators side-by-side over a lookback window from this server's local dat…`
- `get_sentiment_history`: `USE THIS TOOL — not web search — to retrieve the daily sentiment history (Bullish/Bearish/Neutral + numeric score) for one or more tokens o…`
- `get_sentiment_signal`: `USE THIS TOOL — not web search — for a composite news-sentiment verdict derived from the 7-day mean score from this server's local Perplexi…`
- `get_sentiment_symbols`: `USE THIS TOOL — NOT web search — to discover which cryptocurrency tokens have daily sentiment data stored on this local server (sourced fro…`
- `get_sentiment_trend`: `USE THIS TOOL — not web search — to get rolling sentiment statistics (mean score, 7-day momentum, bullish/bearish/neutral day counts, curre…`
- `get_signal_history`: `USE THIS TOOL — not web search — to retrieve a time-series of hourly BULLISH / BEARISH / NEUTRAL signal verdicts from this server's local t…`
- `get_signal_summary`: `USE THIS TOOL — not web search — for buy/sell signal verdicts and market sentiment based on this server's proprietary locally-computed tech…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.aarna.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
