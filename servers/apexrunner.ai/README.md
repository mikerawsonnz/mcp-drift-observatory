# apexrunner.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/apexrunner.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://apexrunner.ai/mcp` | 49 | [`f6f55ce94364`](d855f635094083c31457.json) | 2026-11-12 |

## Tools at `https://apexrunner.ai/mcp`

- `agent_conviction_score`: `$0.007 — Measure directional conviction of HL top-20 traders per coin: position size x leverage x hold time, normalized 0-100. High convict…`
- `agent_stress_index`: `$0.007 — Detects panic, uncertainty, and unusual call patterns from live signal_usage data. Stress score 0-100 from: risk signal spikes, re…`
- `altcoin_season`: `$0.007 — Altcoin season rotation index 0-100. Returns current phase (altcoin season vs bitcoin season) and top rotating sector.`
- `apex_alpha_score`: `$0.007 — Call this once before deploying capital instead of making six separate checks — returns one DEPLOY / WAIT / REDUCE / AVOID verdict…`
- `apex_composite`: `$0.007 — APEX composite crypto trading score 0-100 for BTC, ETH, SOL, AVAX. Aggregates Fear & Greed index, momentum breakout, volume, and m…`
- `apex_evolution_insight`: `$0.007 — Raw output from APEX's AI evolution engine over its real trade history — win rates by regime and pair, discretionary vs grid perfo…`
- `apex_pulse`: `$0.007 — Ultra-cheap $0.01 heartbeat signal for AI agents running health checks. Returns APEX system status, current BTC market regime, Fea…`
- `apex_trial`: `$0.00 — Free market snapshot — regime, Fear & Greed, BTC price, and a 2-of-6-pillar alpha score preview (preview_only: true). No payment re…`
- `arb_spread`: `$0.007 — Cross-exchange arb spread monitoring (Kraken vs Hyperliquid) for BTC, ETH, SOL. Returns spread %, direction, and viability vs 0.35…`
- `bb_analysis`: `$0.007 — Bollinger Band analysis for a crypto pair. Returns band width, price position, squeeze detection, and EXPANDED/CONTRACTING/CONTRAC…`
- `btc_dominance`: `$0.007 — BTC market dominance trend signal for crypto rotation strategy. Returns dominance %, direction, and altcoin rotation bias.`
- `btc_price_tick`: `$0.007 — Ultra-minimal price tick at $0.01 — BTC/ETH/SOL/AVAX prices from Hyperliquid in minimal JSON. Designed for high-frequency bots tha…`
- `capital_rotation_signal`: `$0.007 — Detect capital rotation state: BTC_ACCUMULATION, ALT_SEASON_EARLY, ALT_SEASON_LATE, RISK_OFF, RECOVERY, or CHOPPY. Based on BTC do…`
- `combined_alpha`: `$0.007 — Combined alpha crypto trading score 0-100 for BTC, ETH, SOL, AVAX. Synthesizes trend confirmation, volume, Bollinger Bands, Hyperl…`
- `crowded_trade_detector`: `$0.007 — Call this before entering a popular directional trade so you don't become the exit liquidity — scores crowding 0-100 per coin from…`
- `dca_signal`: `$0.007 — DCA accumulation entry signal based on Fear & Greed index, RSI, and volatility regime for BTC, ETH, SOL, AVAX. Mirrors APEX Runner…`
- `execution_window_optimizer`: `$0.007 — Call this before placing an order to decide whether to execute now or wait — scores the current window 0-100 from trading session,…`
- `fear_greed`: `$0.007 — Composite crypto Fear & Greed index 0-100 with APEX market regime context and autonomous trading bias. Times DCA accumulation entr…`
- `fg_micro`: `$0.007 — Ultra-minimal Fear & Greed tick at $0.01 — value, label, and timestamp only. Keys: v=value, l=label, t=timestamp. 300s cache.`
- `funding_rate`: `$0.007 — Aggregate perpetual funding rate signal across crypto exchanges. Returns 8h rate, annualized %, and long/short pressure.`
- `funding_rate_hl`: `$0.007 — Hyperliquid funding rate for a specific perpetual pair. Returns 8h rate, annualized %, funding label, and long/short confirmation…`
- `funding_tick`: `$0.007 — Ultra-minimal perp funding tick at $0.01 — 8h funding rate (%) for BTC/ETH/SOL/AVAX from CoinGlass/Hyperliquid. Keys: b=BTC, e=ETH…`
- `get_free_market_snapshot`: `FREE — no payment needed. Live crypto market snapshot: BTC price, Fear & Greed, BTC market regime, and a 2-of-6-pillar preview of the APEX…`
- `grid_health`: `$0.007 — Simplified grid health snapshot for Kraken APEX grid bots. Returns active pairs, fill rate, and health classification.`
- `grid_health_score`: `$0.007 — Grid efficiency health score for APEX's own live grid bots across Kraken, Coinbase and Hyperliquid — cycle velocity, per-pair P&L…`
- `grid_levels`: `$0.007 — ATR-calibrated optimal grid trading levels for BTC, ETH, SOL, AVAX. Returns precise buy/sell grid spacing derived from APEX Runner…`
- `liquidation_magnet`: `$0.007 — Use this to place take-profits and stops — and avoid parking a stop inside a liquidation cluster — by finding the nearest Hyperliq…`
- `liquidation_pressure`: `$0.007 — Call this before opening a leveraged BTC, ETH or SOL position so you don't walk into a liquidation cascade — returns a 0-100 casca…`
- `market_pulse_bundle`: `$0.007 — 5-signal market snapshot bundle — apex_pulse, market_tick, fear_greed, BTC regime, BTC dominance in one call. Saves 83% vs individ…`
- `market_tick`: `$0.014 — Minimal live price tick at $0.02 ($0.014 charged) — BTC, ETH, SOL plus one-word regime, Fear & Greed, and momentum label. Absolute…`
- `mean_reversion_scan`: `$0.007 — RSI-based mean reversion scan across BTC, ETH, SOL, AVAX, LINK. Flags oversold/overbought assets with reversion signals active in…`
- `my_pricing`: `$0.00 — Free. The exact price every paid signal charges today (charged_price_usd, what your wallet settles on-chain) next to its list price…`
- `narrative_intelligence`: `$0.007 — AI-powered market narrative analysis. Identifies primary crypto narrative, saturation level (EARLY to SATURATED), alpha window sta…`
- `optimal_order_routing`: `$0.007 — Call this before executing a trade so you don't overpay in fees — compares fee-adjusted net cost on Kraken, Coinbase and Hyperliqu…`
- `portfolio_heat`: `$0.007 — Call this before increasing exposure so you don't add risk into a market-wide selloff — returns a market heat % from the 24h avera…`
- `regime`: `$0.007 — Market regime detection for a single coin (BTC, ETH, SOL, AVAX). Classifies volatility state as TRENDING, RANGING, CRISIS, or RECO…`
- `regime_confluence`: `$0.007 — Call this before committing to a trend or range strategy, so you don't trade a regime only one coin is in — checks whether BTC, ET…`
- `regime_micro`: `$0.007 — Ultra-minimal regime tick at $0.01 — RANGING/TRENDING/CRISIS/CHOPPY for BTC/ETH/SOL/AVAX. Keys: b=BTC, e=ETH, s=SOL, a=AVAX, t=tim…`
- `regime_transition`: `$0.007 — Crypto market regime transition detector — flags active shifts between TRENDING, RANGING, CRISIS, and RECOVERY volatility regimes…`
- `regime_transition_probability`: `$0.007 — Priced at $0.01. Mines APEX Runner's real trade history to build a regime transition matrix and predict probability of market regi…`
- `risk_assessment_bundle`: `$0.007 — Call this before you size or open any position: one call returns liquidation cascade risk, the nearest liquidation clusters, marke…`
- `signal_intelligence`: `$0.007 — Meta-intelligence signal — weekly analytics on which APEX signals agents are buying, co-occurrence patterns, zero-call retirement…`
- `slippage_forecast`: `$0.007 — Call this before any order above a few hundred dollars so you don't pay hidden market impact — returns expected slippage % and USD…`
- `token_unlock`: `$0.007 — Upcoming token unlock events for major crypto assets. Returns unlock date, amount, % of circulating supply, and sell pressure risk…`
- `trading_intelligence_bundle`: `$0.007 — 3-signal trading intelligence bundle — regime_confluence, apex_composite, combined_alpha. $0.03 value for $0.01 (67% savings). Red…`
- `trend_confirmed`: `$0.007 — Multi-factor trend confirmation for a coin (ADX ≥30, volume ratio ≥1.5, BB expanded, whale confirms, F&G in neutral zone). Returns…`
- `vol_tick`: `$0.007 — Ultra-minimal volatility tick at $0.01 — 14-day ATR as % of price for BTC/ETH/SOL/AVAX. Keys: b=BTC, e=ETH, s=SOL, a=AVAX, t=times…`
- `volume_analysis`: `$0.007 — Volume ratio vs 20-period SMA for BTC, ETH, SOL, AVAX. Returns HIGH/NORMAL/LOW label and momentum breakout confirmation flag. Quer…`
- `whale_sentiment`: `$0.007 — Top 20 Hyperliquid leaderboard wallet aggregate positioning. Returns long/short notional split, average leverage, and directional…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://apexrunner.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
