# infrapulse.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/infrapulse.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://infrapulse.ai/mcp/core` | 6 | [`1888394daf25`](a75e7800d34b940be074.json) | 2026-08-20 |
| `https://infrapulse.ai/mcp` | 6 | [`22ab17efb7d0`](a784d85e70b62db7ac7d.json) | 2026-08-24 |

## Tools at `https://infrapulse.ai/mcp/core`

- `authorize`: `Create an idempotent prepaid authorization for a quoted operation. This may reserve private account credits but does not execute provider w…`
- `connect`: `Create, inspect, or explicitly approve a private OAuth-bound InfraPulse connection. OAuth proves owner identity; requested InfraPulse opera…`
- `discover`: `Discover InfraPulse production capabilities and the universal execution contract without changing account state.`
- `execute`: `Execute authorized provider work through InfraPulse. Requires a stable request_id and canonical authorization_id; may consume prepaid credi…`
- `quote`: `Get a deterministic price quote before authorization or execution. This does not reserve credits or run provider work.`
- `verify_receipt`: `Verify an InfraPulse signed receipt by receipt_id or receipt object without changing account or provider state.`

## Tools at `https://infrapulse.ai/mcp`

- `authorize`: `Create an idempotent prepaid authorization for a quoted operation. This may reserve private account credits but does not execute provider w…`
- `connect`: `Create, inspect, or explicitly approve a private OAuth-bound InfraPulse connection. OAuth proves owner identity; requested InfraPulse opera…`
- `discover`: `Discover InfraPulse production capabilities and the universal execution contract without changing account state.`
- `execute`: `Execute authorized provider work through InfraPulse. Requires a stable request_id and canonical authorization_id; may consume prepaid credi…`
- `quote`: `Get a deterministic price quote before authorization or execution. This does not reserve credits or run provider work.`
- `verify_receipt`: `Verify an InfraPulse signed receipt by receipt_id or receipt object without changing account or provider state.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://infrapulse.ai/mcp/core"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
