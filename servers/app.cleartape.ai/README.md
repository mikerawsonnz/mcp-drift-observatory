# app.cleartape.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.cleartape.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.cleartape.ai/mcp` | 11 | [`29abe499003e`](36157844829181a9ecb6.json) | 2026-10-16 |

## Tools at `https://app.cleartape.ai/mcp`

- `calculate_atr_stop`: `A volatility (ATR) stop: entry minus (long) or plus (short) a multiple of the average true range. Give atr, or at least five recent daily r…`
- `calculate_drawdown_recovery`: `The gain needed to recover from a drawdown and, optionally, how many losing trades in a row at a fixed risk per trade cause it. Computed wi…`
- `calculate_expectancy`: `Expectancy per trade, per 100 trades, payoff ratio, break-even win rate and profit factor from a win rate and average win and loss. Compute…`
- `calculate_kelly_criterion`: `Full and fractional Kelly risk per trade from a win rate and payoff ratio, with the edge per 1R and the break-even win rate. Computed with…`
- `calculate_losing_streak`: `The exact probability of at least one losing streak of a given length over a number of independent trades, the expected longest streak and…`
- `calculate_position_size`: `Position size from the stop: how many shares to buy (or short) so that a stop-out loses a set percentage of the account. Computed with the…`
- `calculate_risk_reward`: `Risk/reward ratio of a planned trade, the win rate it needs to break even, and (optionally) an exit expressed as an R multiple. Computed wi…`
- `calculate_trading_cost`: `The cost of one round trip (commissions, bid-ask spread, slippage) in USD, in R, as a share of the target move and of the position, and ove…`
- `get_trading_system_rules`: `Without id: lists Clear Tape's eleven preset trading systems (trend, breakout, momentum and volume) with their style, holding period and on…`
- `lookup_glossary_term`: `Looks up a trading term in Clear Tape's bilingual (English and Simplified Chinese) glossary of about 70 terms, such as "R multiple", "ATR",…`
- `search_learning`: `Searches Clear Tape's free trading education by keyword: the Learn articles, the Academy lessons, the trading-strategy pages and the calcul…`

## Changes

- 2026-10-16: [description changed, schema changed](../../deltas/2026-10-16/36157844829181a9ecb6.json): `7 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.cleartape.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
