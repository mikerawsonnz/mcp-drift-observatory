# agents.avasis.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agents.avasis.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agents.avasis.ai/mcp` | 3 | [`e82dd8e13813`](13be9a5c0441e3f603e0.json) | 2026-11-17 |

## Tools at `https://agents.avasis.ai/mcp`

- `research_pack`: `Get a deterministic due-diligence report with evidence for every claim and explicit coverage gaps. Paid HTTP offer: $5.00 USDC. This tool r…`
- `token_verdict`: `Screen a token's structural risks before investigating a trade. Paid HTTP offer: $0.02 USDC. This tool returns free x402 payment requiremen…`
- `wallet_risk`: `Check a counterparty's known risk signals and recent USDC flows before interacting. Paid HTTP offer: $0.02 USDC. This tool returns free x40…`

## Changes

- 2026-11-17: [count changed, tool added, tool removed](../../deltas/2026-11-17/13be9a5c0441e3f603e0.json): `3 tool(s) added; 4 tool(s) removed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agents.avasis.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
