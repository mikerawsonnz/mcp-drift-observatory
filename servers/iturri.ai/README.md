# iturri.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/iturri.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://iturri.ai/mcp` | 22 | [`f806ddd27434`](e5e08d17256378eec939.json) | 2026-08-23 |

## Tools at `https://iturri.ai/mcp`

- `audit_my_data`: `FREE: submit YOUR OHLCV bars and get an accuracy verdict against the verified archive — score, worst windows, systematic-offset findings. T…`
- `build_bundle`: `Signed URL for a dataset SKU. Packs: crypto/equities ($59 each), everything ($149: both packs + all token sequences, $730 list), tokens ($1…`
- `describe_catalog`: `Free discovery: symbols, timeframes, ranges, pricing, quality legend.`
- `get_bars`: `Quality-flagged OHLCV candles. Priced per 1,000 candles.`
- `get_context`: `Context series: fear_greed_1d, VIX_1d, DXY_1d, TNX_1d, DJI_1d.`
- `get_events`: `Curated macro/crypto events (FOMC w/ surprise, halvings, incidents) in a range.`
- `get_features`: `Documented leakage-safe feature matrix rows. Priced per call.`
- `get_fundamentals`: `Point-in-time SEC XBRL fundamentals (80 filers, incl. delisted): every restatement vintage with its filed date. Pass as_of for what was kno…`
- `get_funding`: `Perp funding-rate settlement history from listing date (checksummed archive).`
- `get_funding_spread`: `Hourly CEX-vs-DEX funding spread (67 symbols): Hyperliquid funding vs Binance 1h-equivalent, from HL genesis 2023-05.`
- `get_insider`: `SEC Form 4 insider transactions as filed (80 symbols, since 2016): officer/director trades with shares, price, post-trade holdings.`
- `get_institutional`: `Quarterly 13F institutional aggregates (81 symbols): holders, shares, value + QoQ deltas from SEC DERA structured tables.`
- `get_long_short`: `Positioning ratios at 5-minute cadence from the checksummed venue archive (2020-09+): top-trader long/short by accounts and by position siz…`
- `get_market_pulse`: `FREE daily pulse across the catalog: regime flips, funding extremes, CEX-vs-DEX spread extremes, biggest daily moves. One day of values — t…`
- `get_open_interest`: `Open interest with per-row quality flags (verified archive + flagged bridge). tf=1h (default, full history) or tf=5m (archive-native 5-minu…`
- `get_orderflow`: `Taker buy/sell imbalance, trade counts, quote volume (1h/1d via API; denser tiers in packs). buy_ratio 0.5 = balanced.`
- `get_quality_receipts`: `FREE public scoreboard: last 30 daily fresh-data audits (cross-venue in-band vs Coinbase, 1m->1h rebuild exactness, depth sanity) — failure…`
- `get_regime_label`: `Descriptive market-state label (trend/range × calm/vol quadrant) for the most recent completed bar at or before a timestamp. Not a predicti…`
- `get_whats_new`: `FREE: what the daily refresh changed — dataset windows extended vs ~7 days ago, new symbols and sections, freshness per asset class.`
- `lookahead_check`: `FREE: submit backtest signals ({t, price}) and get an execution-feasibility verdict — impossible fills outside the bar's traded range, fill…`
- `survivorship_check`: `FREE: submit a backtest universe + window and get a survivorship-bias verdict — which of your symbols died mid-window, and which delisted s…`
- `validate_backtest_data`: `Quality report for a dataset spec before you backtest on it: coverage, per-bar quality distribution, gaps, and concrete warnings.`

## Changes

- 2026-08-23: [count changed, description changed, schema changed, tool added](../../deltas/2026-08-23/e5e08d17256378eec939.json): `1 tool(s) added; 4 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://iturri.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
