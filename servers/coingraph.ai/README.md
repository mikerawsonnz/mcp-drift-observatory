# coingraph.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/coingraph.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://coingraph.ai/api/mcp` | 22 | [`e811b79dbeb9`](8e38f137a38da246adbf.json) | 2026-10-24 |

## Tools at `https://coingraph.ai/api/mcp`

- `ask_about_token`: `Ask CoinGraph anything about a token, or test whether a statement is true. A 'question' gets a plain answer with key points and their evide…`
- `check_token`: `The check to run before acting on a token. Returns a verdict — proceed, caution or avoid — rated across momentum, liquidity, leverage, onch…`
- `get_market_overview`: `The whole crypto market at a glance: total market cap and volume, BTC and ETH dominance, sectors, how many tokens are up or down, Fear & Gr…`
- `get_proof`: `Proof of exactly what CoinGraph told you. Give the id of a check (eval_…), an answer (ans_…), an agent run (run_…) or a brief (a number) an…`
- `get_service_status`: `Is CoinGraph working right now? Shows whether data collection is healthy, how fresh each data source is, what is covered (tokens, exchanges…`
- `get_token_brief`: `Why did this token move? Returns CoinGraph's brief: a headline, what happened, the likely causes with confidence, the onchain evidence (wha…`
- `get_token_snapshot`: `Everything CoinGraph knows about a token right now, in one answer: price and market data, liquidity and order-book depth, futures (open int…`
- `get_token_timeline`: `What happened to a token over time. Charts: price, 1-minute candles, open interest, funding, long/short ratios, exchange net flow, exchange…`
- `get_track_record`: `CoinGraph's public scorecard. Every check, signal and brief it issued, what it said, what the price did 1 hour, 24 hours and 7 days later,…`
- `lookup_address`: `Who is behind a blockchain address? Returns its label (an exchange such as Binance, a contract, a burn address, or unlabelled), a screening…`
- `run_alert_watchtower`: `Watches your tokens and explains every alert. Give it a list of tokens and optionally a webhook URL. It returns what is happening right now…`
- `run_daily_market_brief`: `The whole market in one readable page. Opens with CoinGraph's own record from the last 24 hours (what followed each check), then the market…`
- `run_due_diligence_analyst`: `A full due-diligence memo on any token in one run. Structured like exchange listing reviews (Coinbase, Kraken) and lending-risk onboarding…`
- `run_leverage_radar`: `Spots crowded futures trades before they unwind. Scores every token with a futures market from 0 to 100 for crowding, combining funding aga…`
- `run_opportunity_scout`: `Finds what's moving, keeps only what's safe to act on. Scans the 100 tracked tokens for momentum, volume spikes, coins leaving exchanges an…`
- `run_portfolio_checkup`: `A health check for everything in a wallet. Reads a wallet's holdings live from the chain, runs the CoinGraph check on each tracked token, a…`
- `run_trade_gatekeeper`: `The check every trade passes before it is placed. Give it a token, an order size and optionally your rules. It runs the CoinGraph check, me…`
- `run_treasury_steward`: `Enforces the treasury's rules, with proof. Give it the treasury's assets and its investment policy (minimum liquidity, maximum holder conce…`
- `run_wallet_guard`: `Checks a swap or a send before you sign it. Before a swap, it checks the token: contract risks (honeypot, taxes, mint/freeze/blacklist powe…`
- `run_whale_watch`: `Shows what the big wallets are doing with a token. Reads onchain flows through NOWNodes: large transfers tagged with exchange names, net fl…`
- `search_tokens`: `Find a token. With no input, lists the 100 tokens CoinGraph tracks with price, 1h and 24h change, open signals and the latest headline. Wit…`
- `watch_tokens`: `Watch up to 50 tokens and get told when something important happens. CoinGraph sends a signed message to your webhook URL when a signal fir…`

## Changes

- 2026-10-24: [description changed](../../deltas/2026-10-24/8e38f137a38da246adbf.json): `1 field(s) changed`
- 2026-10-20: [count changed, tool added, tool removed](../../deltas/2026-10-20/8e38f137a38da246adbf.json): `22 tool(s) added; 14 tool(s) removed; signals: credential_shaped_string_introduced` **(notable)**
- 2026-09-22: [description changed](../../deltas/2026-09-22/8e38f137a38da246adbf.json): `2 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://coingraph.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
