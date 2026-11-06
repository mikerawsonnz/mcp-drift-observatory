# x402-services-production.up.railway.app: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/x402-services-production.up.railway.app.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://x402-services-production.up.railway.app/mcp` | 159 | [`a8931e31a79b`](784c267ced76f24cc305.json) | 2026-08-20 |

## Tools at `https://x402-services-production.up.railway.app/mcp`

- `agent_reputation`: `Agent/wallet reputation score (0-100): a portable on-chain trust signal — activity, holdings, counterparty diversity, and sanctions — with…`
- `ai_chat`: `LLM chat completion via x402 - no accounts, no API keys. Fast models (gpt-4o-mini, gemini-2.0-flash, llama-3.3-70b, mistral-small, deepseek…`
- `ai_chat_pro`: `Frontier-model chat completion via x402 (gpt-4o, claude-sonnet-4, gemini-2.5-pro, deepseek-r1, grok-3). OpenAI-compatible messages. Payable…`
- `ai_models`: `AI Gateway model list: available LLMs per tier with prices and caps. The FIRST LLM inference gateway payable in USDG on Robinhood Chain (al…`
- `analytics_indicators`: `Technical indicators for a token computed from daily closes: RSI(14), SMA20/50, EMA12/26, MACD, with bullish/bearish signals. Send { coin,…`
- `analytics_ohlcv`: `OHLCV candles for a DEX pool (open/high/low/close/volume) at minute/hour/day resolution. Send { chain, pool, timeframe?, limit? }. Charting…`
- `analytics_price_at`: `Point-in-time historical price: what did a token cost at a past date/timestamp? Send { coin, when }. Essential for backtesting, accounting,…`
- `board_get`: `Shared blackboard: read one key or list all keys+entries. Send { board, token, key? }. [x402 paid tool — price $0.003; POST /api/board/get]`
- `board_set`: `Shared blackboard: set a versioned key on a multi-writer board. Send { board, token, key, value }. [x402 paid tool — price $0.003; POST /ap…`
- `business_days`: `Add/subtract business days (skips weekends + given holidays). Send { start?, addDays, holidays?, timezone? }. [x402 paid tool — price $0.00…`
- `calc`: `Exact calculator + unit conversion (arbitrary precision). e.g. '3 inch to cm', 'sqrt(2)^10'. Send { expression, precision? }. [x402 paid to…`
- `catalysts_calendar`: `Upcoming token-unlock calendar: the biggest unlocks across a basket of tokens within N days, ranked by USD value. Send { protocols?, days?…`
- `catalysts_governance`: `On-chain governance activity via Snapshot: active (or recent) proposals ranked by voting power, with title, space, votes, and end time. Sen…`
- `catalysts_search`: `Find protocols that have tracked token-unlock schedules, by name substring. Send { query }. Use the returned slug with catalysts/unlocks. […`
- `catalysts_unlocks`: `Token unlock / vesting schedule for a protocol: next unlock date, token amount, USD value, category and type, plus upcoming events. Send {…`
- `compliance_label`: `Entity labeling: is this address an EOA, a (proxy) contract, a known protocol, or flagged as scam — with name and public tags. Send { addre…`
- `compliance_risk`: `Address risk score (0-100): OFAC status, interaction with sanctioned addresses, contract verification, and activity, with a risk level and…`
- `compliance_screen`: `OFAC sanctions screening: is this address on the US OFAC sanctioned-address list? Send { address }. Every agent moving money legally needs…`
- `compliance_taint`: `Tainted-funds tracing: does this wallet's incoming money trace back to a sanctioned address within N hops? Multi-hop fund-flow trace on Bas…`
- `counter`: `Atomic counter: increment-and-return a named counter (collision-free running totals & IDs across agent runs). Send { name, token, by? }. [x…`
- `cron_explain`: `Explain a cron expression: the next N run times in a timezone. Send { expression, count?, timezone? }. [x402 paid tool — price $0.003; POST…`
- `crypto_activity`: `Wallet activity summary: recent transactions, top methods called, distinct counterparties, and latest actions for an address on Base. Send…`
- `crypto_balances`: `Full wallet portfolio: native ETH + all ERC-20 token balances for an address on Base, with amounts. Send { address }. Let agents read any w…`
- `crypto_contract`: `Contract decoder: pass a verified 0x contract address to get its function ABI, or a 0x-selector (8 hex) to decode which function it is. Sen…`
- `crypto_convert`: `Convert an amount between any two crypto/fiat assets at live rates. Send { amount, from, to }, e.g. convert 1.5 ETH to USDC. Instant FX for…`
- `crypto_ens`: `Resolve an ENS name or Basename to an address, or reverse-resolve a 0x address to its name + avatar. Send { input }. Human-readable identit…`
- `crypto_gas`: `Live Base gas oracle: current gas price plus estimated cost (ETH & USD) for a transfer, swap, or mint. Send {} — no input needed. Agents bu…`
- `crypto_price`: `Live crypto & token prices in USD. Send tickers or coingecko ids, e.g. { symbols: ["ETH","USDC","BTC"] }. Real-time on-chain pricing for fi…`
- `crypto_token`: `Token intelligence: name, symbol, supply, holder count, source-verification, and safety signals for a contract. Send { address }. Agents ve…`
- `crypto_tx`: `Transaction status & receipt on Base: confirmations, success/fail, from/to, value, fee, method. Send { hash }. Agents confirm their on-chai…`
- `crypto_yields`: `Top DeFi yield opportunities across chains from DeFiLlama, filterable by chain/project/min-TVL, ranked by APY. Send { chain?, project?, min…`
- `datetime`: `Date/time math + timezones. op: now / convert / add / diff. Send { op, time?, timezone?, amount?, unit?, to? }. [x402 paid tool — price $0.…`
- `deadman_ping`: `Dead-man's switch: heartbeat to keep the switch from firing. Send { id, token }. [x402 paid tool — price $0.003; POST /api/deadman/ping]`
- `deadman_register`: `Dead-man's switch: if you don't ping within intervalSec, we POST your webhook. Detects crashed agents. Send { id, token, url, intervalSec }…`
- `diff`: `Structured deep diff of two JSON values (added/removed/changed by path). Send { a, b }. [x402 paid tool — price $0.003; POST /api/diff]`
- `escrow_create`: `Create an agent-to-agent conditional-payment agreement: payer, payee, amount, release condition, deadline — returns an id both parties trac…`
- `escrow_list`: `List conditional-payment agreements for your token (yours) or a party address (involving that address). Send { token } or { party }. [x402…`
- `escrow_resolve`: `Resolve a conditional-payment agreement: the creator marks 'release' (pay payee) or 'refund' (return to payer); returns a settlement instru…`
- `escrow_status`: `Check the state of a conditional-payment agreement (pending/released/refunded/expired). Send { id }. [x402 paid tool — price $0.005; POST /…`
- `exec_gas`: `Live gas prices across major chains (Base, Ethereum, Arbitrum, Optimism, Polygon, BSC) with estimated USD cost of a swap. Send { chains? }.…`
- `exec_quote`: `Best-route swap quote across DEXes (KyberSwap aggregator): expected output, USD in/out, price impact %, gas cost, and the DEXes routed thro…`
- `exec_sandwich`: `Sandwich / MEV risk score for a planned swap, from price impact and trade size, with concrete mitigations (private RPC, tighter slippage, o…`
- `exec_slippage`: `Recommended max slippage for a planned swap based on live price impact plus a buffer, with a rating. Send { chain, tokenIn, tokenOut, amoun…`
- `extract`: `Extract structured data (title, links, meta, headings, text) from HTML as JSON. [x402 paid tool — price $0.003; POST /api/extract]`
- `idempotency`: `Idempotency key: returns firstTime:true only once per key within ttl (dedupe retries/double-sends). Send { key, token, ttlSec? }. [x402 pai…`
- `inbox_create`: `Webhook inbox: get a disposable URL that captures inbound POSTs for you to poll. Send { token }. [x402 paid tool — price $0.003; POST /api/…`
- `inbox_poll`: `Webhook inbox: fetch captured messages newer than a timestamp. Send { id, token, since? }. [x402 paid tool — price $0.003; POST /api/inbox/…`
- `jsonschema`: `Validate data against a JSON Schema (strict). Returns valid + detailed errors. Send { schema, data }. [x402 paid tool — price $0.003; POST…`
- `lending_health`: `Aave v3 position health: health factor, collateral, debt, liquidation buffer, and a risk verdict for a wallet. Send { address, chain? }. Kn…`
- `lending_liquidations`: `Liquidation-opportunity scanner: at-risk Morpho Blue borrower positions (health factor < 1) that can be liquidated for a bonus, with borrow…`
- `lending_rates`: `Best supply/lending APYs for an asset across Aave, Compound, Morpho, Spark and more, ranked by yield with TVL. Send { asset, chain? }. Rate…`
- `links_check`: `Batch link-liveness: check up to 50 URLs return 200 (dead-link detection). Send { urls: [..] }. [x402 paid tool — price $0.003; POST /api/l…`
- `lock_acquire`: `Distributed lock: acquire a named lock for ttlSec so only one agent proceeds. Returns acquired:false if held. Send { name, token, ttlSec? }…`
- `lock_release`: `Release a distributed lock you hold. Send { name, token, holder? }. [x402 paid tool — price $0.003; POST /api/lock/release]`
- `markdown`: `Convert raw HTML to clean, LLM-ready markdown. Strips nav/script/style noise. [x402 paid tool — price $0.003; POST /api/markdown]`
- `memory_get`: `Agent Memory: read a stored value by key, or omit key to list all keys in your namespace. Send { ns, token, key? }. [x402 paid tool — price…`
- `memory_set`: `Agent Memory: durable key-value storage that survives between agent runs. Write a JSON value (16KB max) under a key. First write to a names…`
- `options_chain`: `Full options chain for a currency & expiry: per-strike calls & puts with mark price, implied volatility, and open interest. Send { currency…`
- `options_greeks`: `Black-Scholes option pricing: fair value + full greeks (delta, gamma, vega, theta, rho) for ANY option, listed or not. Send { type, spot, s…`
- `options_maxpain`: `Max-pain strike + put/call open-interest ratio for an expiry — the price level where option holders lose most; a positioning/magnet signal.…`
- and 99 more in [784c267ced76f24cc305.json](784c267ced76f24cc305.json)

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://x402-services-production.up.railway.app/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
