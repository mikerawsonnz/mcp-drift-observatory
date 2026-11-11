# mcp.agentgates.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.agentgates.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.agentgates.ai/compute` | 3 | [`e136999eb934`](8e123eb71203886e049b.json) | 2026-11-11 |

## Tools at `https://mcp.agentgates.ai/compute`

- `compute_docs`: `Returns the Agentgates compute docs, read live (markdown written for an agent to follow in one pass): the plans with live prices, how to pa…`
- `compute_plans`: `Lists the confidential virtual machines (Intel TDX, memory encrypted in use) Agentgates rents to agents by the hour: each plan's vCPU, memo…`
- `compute_quote`: `Gets the exact price of one machine without paying: sends the create request with no payment and returns the API's HTTP 402 offer, one leg…`

## Changes

- 2026-11-11: [schema changed](../../deltas/2026-11-11/8e123eb71203886e049b.json): `7 field(s) changed`
- 2026-11-07: [description changed, schema changed](../../deltas/2026-11-07/8e123eb71203886e049b.json): `7 field(s) changed`
- 2026-11-06: [description changed, schema changed](../../deltas/2026-11-06/8e123eb71203886e049b.json): `47 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.agentgates.ai/compute"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
