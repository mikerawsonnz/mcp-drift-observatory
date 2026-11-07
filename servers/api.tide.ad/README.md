# api.tide.ad: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.tide.ad.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.tide.ad/mcp` | 38 | [`875b828aa141`](cf57e535ac93234bd658.json) | 2026-11-07 |

## Tools at `https://api.tide.ad/mcp`

- `address_kind`: `Tell what an address is: a plain key (ed25519, secp256k1, secp256r1), a passkey, a zkLogin address (with its provider), a multisig (members…`
- `agent_pass_precheck`: `Before building: check one action against an Agent Pass's rules as they stand now (active, signer is the agent, rule for the coin or pair,…`
- `agent_pass_report`: `A report for a human on Agent Pass (Sui's on-chain agent authorization): for an owner, an agent or one pass, each pass's status, its rules…`
- `agent_wallet`: `Is this address an AI agent, who does it act for and under what limits (Agent Pass, sui::allowance, Sui Agent Payments grant, t2000, Talus)…`
- `agents_overview`: `The agent world on Sui: agent wallets active in 24 hours, their transactions and volume, Agent Passes, sui::allowance spend, Sui Agent Paym…`
- `balance_at`: `The exact balance a wallet held at a past time or checkpoint, read from full history. With coin, that coin's balance and the transaction th…`
- `billing_status`: `Your credits: what the plan has left this month, prepaid credits bought with USDC, the rate ($3 per million credits, so 1 USDC buys 333,333…`
- `billing_topup`: `Build an unsigned transaction that pays USDC on Sui to tide's treasury for credits ($3 per million credits; 1 USDC buys 333,333). Returns b…`
- `build_transaction`: `Build an unsigned Sui transaction for an action and get it back already checked: tide adds the protocol's own calls, picks the sender's gas…`
- `candles`: `OHLCV price candles for a coin, in USD. Pick interval and an optional from and to. Example: { coin: "SUI", interval: "1h" }.`
- `checkpoint`: `One checkpoint by sequence number, or the newest with seq "latest": time, epoch, gas totals and its transactions as one-line sentences. Use…`
- `confirm_execution`: `After execution: give the executed digest and the receipt (its id, or the receipt object). tide reads the transaction from the chain and co…`
- `docs`: `Search the tide API docs for the method that answers a question, with its parameters, credits and a curl example. Use it when no other tool…`
- `events`: `List on-chain events by Move event type or by package, newest first, with an optional time or checkpoint range. Page with cursor. Example:…`
- `explain_transaction`: `Explain one Sui transaction in plain English: what happened, the steps, who gained or lost which coins (with USD), the fee and the status.…`
- `explain_unsigned`: `Check a Sui transaction before signing it: tide simulates it, explains what it would do in plain words, and checks every recipient, coin an…`
- `get_object`: `Read any Sui object by id: type, owner, version and fields, with its recent change history (which transactions changed it). Example: { id:…`
- `get_object_at`: `Read a Sui object as it was at a version, checkpoint or time: its fields and owner then, or whether it was deleted or wrapped. Use it for w…`
- `nfts`: `The NFTs and kiosk items an address owns: name, collection, image and listing state. Page with cursor. Example: { address: "example.sui" }.`
- `object_children`: `List the dynamic fields of an object with decoded names and values (tables, bags, kiosks, pools, registries), or with depth 1 to 3, its tre…`
- `order_book`: `DeepBook order books. With nothing: every pool with best bid, ask and 24h volume. With pool: its depth and latest trades. With address: the…`
- `owner_agents`: `The AI agents one address runs on Sui: Agent Passes, allowances it granted, Sui Agent Payments grants, t2000 wallets it funded and agent wa…`
- `package_info`: `A Move package. With only id: its modules, functions and upgrade history. With module and function: how to call it, each parameter explaine…`
- `perp_market`: `One perpetual futures market on Sui (Aftermath, Bluefin or Parchment): mark and index price, 24h change and volume, open interest, funding…`
- `price`: `USD prices for up to 50 coins, now or at a past time. Pass coin types or symbols. Example: { coins: ["SUI", "DEEP"] }.`
- `receipt_for_transaction`: `Before you sign: send the exact unsigned bytes and your intent; tide dry-runs them on mainnet and returns a receipt signed by tide (ed25519…`
- `search`: `Find anything on Sui by text: coins by symbol or name, SuiNS names, perps markets, pools, packages, addresses, objects and digests. Returns…`
- `sql`: `Run one SQL SELECT over every Sui transaction, event, object version and balance change since genesis. Needs an API key. Returns up to 100…`
- `staking`: `With address: the wallet's staked SUI, per stake its validator, principal, rewards and status. With validator: that validator's stake, comm…`
- `token_info`: `A coin's price, market cap, liquidity, volume and holder count, its safety checks (mint authority, deny list, concentration), its top 10 ho…`
- `trace_funds`: `Follow money between addresses. direction in: who sent funds to this address, hop by hop back, plus who first funded it. out: where its fun…`
- `verify_receipt`: `Check a receipt's ed25519 signature against tide's published key (https://api.tide.ad/.well-known/tide-attest.json), that its id matches it…`
- `wallet_history`: `A wallet's transactions since genesis, newest first, each as one decoded sentence with the coins in and out. Filter by coin, direction (in…`
- `wallet_profile`: `Everything about a wallet in one call: total value with price status, top coins, DeFi and launchpad positions, SuiNS names and labels, who…`
- `walrus_blob`: `Everything about one Walrus blob: status (registered, certified, expired, deleted), owner and uploader, size, the register and certify tran…`
- `withdraw_plan`: `List a wallet's staking, liquid staking and lending positions (native stakes, afSUI, haSUI, vSUI, sSUI, stSUI, Suilend, NAVI, Scallop), eac…`
- `yield_options`: `Every place on Sui to earn yield (lending, pools, liquid staking, native staking) with the APY each actually paid over 7 and 30 days, depos…`
- `yield_plan`: `A ranked menu of 3 to 6 yield options on Sui for an amount: the realized APY used (never the advertised one), expected USD over the horizon…`

## Changes

- 2026-11-07: [description changed, schema changed](../../deltas/2026-11-07/cf57e535ac93234bd658.json): `3 field(s) changed`
- 2026-11-06: [count changed, tool added](../../deltas/2026-11-06/cf57e535ac93234bd658.json): `1 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.tide.ad/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
