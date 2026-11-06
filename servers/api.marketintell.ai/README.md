# api.marketintell.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.marketintell.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.marketintell.ai/mcp` | 17 | [`01ab1e6a61cf`](ce5f2450e60feaa87c7e.json) | 2026-08-20 |

## Tools at `https://api.marketintell.ai/mcp`

- `alpha_signals`: `Fetch recent alpha signals — automated market intelligence. Crypto signals every ~10 min; equities (Beta) every ~30 min during US market ho…`
- `billing_status`: `Return the authenticated key's plan, daily quota usage, monthly LLM-cost-cents, and cap. Mirrors GET /v1/billing/status.`
- `chat`: `Run a query through MarketIntell's brain (auto-routes to T1 fast agent or T2 CoT pipeline based on intent). Returns synthesized analysis wi…`
- `chat_deep`: `Run a query through MarketIntell's T3 supervisor — parallel specialists across technical/derivatives/macro/social/onchain/etc. plus synthes…`
- `execute_approve_intent`: `Approve a pending trade intent and place the order at the broker. Returns the executed_order audit row. Requires 'trade' scope.`
- `execute_list_intents`: `List the caller's recent trade intents (pending, executed, rejected). Requires 'trade' scope.`
- `execute_propose_intent`: `Propose a trade intent to the user's connected broker. Writes a pending row the user reviews + approves. Requires 'trade' scope. Use this w…`
- `execute_read_portfolio`: `Read the caller's connected broker account snapshot — equity, cash, buying power, open positions. Requires 'trade' scope.`
- `health`: `MarketIntell system health — uptime, cache stats, memory, provider circuit-breaker states.`
- `portfolio_analyze`: `Compute PnL + risk assessment for a portfolio you own. Returns per-holding pnl, risk_assessment, and top_risks.`
- `portfolio_create`: `Create a new portfolio for the authenticated key. Holdings are token symbol + amount (+ optional entry_price and notes).`
- `portfolio_list`: `List all portfolios owned by the authenticated key. Returns id, name, holdings, timestamps.`
- `register`: `Step 2 of MCP self-signup. Submit the challenge id + solved nonce to provision a fresh Free-tier API key. The key is shown ONCE — store it.…`
- `register_challenge`: `Step 1 of MCP self-signup. Returns a proof-of-work challenge. Solve locally (find a nonce whose sha256 has the required leading zero hex ch…`
- `screener`: `Token screening — find trending tokens, top gainers, and top losers. Use this to discover what's moving in the market right now.`
- `sessions_list`: `List the authenticated key's recent chat sessions. Useful to resume prior conversations.`
- `signal_performance`: `Realized signal accuracy — rolling 30-day win rate over CLOSED trade signals, where a win is a real take-profit / in-profit expiry (net pos…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.marketintell.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
