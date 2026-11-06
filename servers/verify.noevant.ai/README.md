# verify.noevant.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/verify.noevant.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://verify.noevant.ai/mcp` | 5 | [`06c0741b44c3`](50be926a4adf36c97f2d.json) | 2026-08-20 |

## Tools at `https://verify.noevant.ai/mcp`

- `check_usage`: `Report how many verifications remain on this account for the current period.`
- `estimate_claims`: `FREE. Break text into checkable claims and report how many there are and how many credits verifying them would cost. Spends nothing and ver…`
- `recall_claim`: `Look up whether a claim has already been verified on this account, without spending a verification.`
- `top_up`: `Buy more verification credits without leaving the conversation. Call with confirm false (or omit it) to see the price, the card on file and…`
- `verify_claims`: `Fact-check text against live web evidence from two independent retrievers, then have a model from a different lab audit the verdict. Return…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://verify.noevant.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
