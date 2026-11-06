# mcp.djzs.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.djzs.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.djzs.ai/mcp` | 4 | [`406895a08e48`](6add31b600e24a0d44ef.json) | 2026-09-14 |

## Tools at `https://mcp.djzs.ai/mcp`

- `query_agent_trust`: `Query an agent's DJZS trust score, aggregated on-chain (Base mainnet) from its audit history and indexed via the DJZS subgraph. USE BEFORE…`
- `query_pol_certificates`: `Query immutable ProofOfLogic certificates stored on Irys Datachain by DJZS Protocol. USE THIS TOOL when you need to verify audit history fo…`
- `verify_perp_trade`: `Deterministic pre-execution audit of a perpetual or spot TRADE thesis (direction, size, leverage, entry, stop, target, venue, and the REASO…`
- `verify_pm_trade`: `Deterministic pre-execution audit of a prediction-market trade thesis, run before capital is committed. USE THIS TOOL before opening, sizin…`

## Changes

- 2026-09-14: [description changed, schema changed](../../deltas/2026-09-14/6add31b600e24a0d44ef.json): `15 field(s) changed; signals: length_more_than_doubled`
- 2026-09-09: [count changed, tool added](../../deltas/2026-09-09/6add31b600e24a0d44ef.json): `1 tool(s) added`
- 2026-08-30: [description changed, field changed](../../deltas/2026-08-30/6add31b600e24a0d44ef.json): `2 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.djzs.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
