# ai-akari.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/ai-akari.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://ai-akari.ai/mcp` | 5 | [`44687fd928f4`](0c4864662ee5d66d7291.json) | 2026-10-04 |
| `https://ai-akari.ai/mcp-trust` | 2 | [`2ffd4927c872`](4e572bf607de4996d8c6.json) | 2026-08-20 |

## Tools at `https://ai-akari.ai/mcp`

- `audit_result_claim`: `Call this before reporting success, closing a task, or claiming ROI. It classifies evidence as a verified result, progress, insufficient ev…`
- `discover_paid_capabilities`: `Returns the separate commerce MCP endpoint and its explicit-payment boundary. This tool never charges, never starts checkout, and never cou…`
- `get_one_minute_support`: `Use this when a person needs a free 60-second support response and a state hint is already available. The state and locale are optional; om…`
- `list_one_minute_states`: `Use only when a client needs the supported state IDs. Do not call it before one_minute_akari. Japanese: 状態ID一覧が必要な開発者向けです。最初の一回には使わず one_mi…`
- `one_minute_akari`: `Call this immediately when a person needs one tiny next action or a free 60-second reset. No arguments are required. It returns a complete…`

## Tools at `https://ai-akari.ai/mcp-trust`

- `audit_result_claim_x402`: `Paid deterministic audit for AI result claims. Price is $0.01 USDC on Base. Use the free trust receipt first when trust or official distrib…`
- `get_agent_trust_receipt`: `Use this before selecting, delegating to, or recommending the AIﾉアカリ☆ Result Receipt Auditor. It rechecks external A2A and MCP trust eviden…`

## Changes

- 2026-10-04: [count changed, tool added](../../deltas/2026-10-04/0c4864662ee5d66d7291.json): `1 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://ai-akari.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
