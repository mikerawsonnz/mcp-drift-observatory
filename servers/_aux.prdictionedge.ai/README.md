# _aux.prdictionedge.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/_aux.prdictionedge.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://aux.prdictionedge.ai/mcp/v1` | 2 | [`389a49bae13a`](f0bc295a8caaf4fbfad9.json) | 2026-08-20 |

## Tools at `https://aux.prdictionedge.ai/mcp/v1`

- `aux_mortgage_closing_preflight`: `Evaluate one published fictional mortgage closing scenario for destination changes and cash-to-close evidence sufficiency. Optionally add l…`
- `aux_transaction_preflight`: `Evaluate a purpose-built synthetic B2B payment scenario for duplicate invoices, changed payment destinations, vendor-history anomalies, and…`

## Changes

- 2026-08-20: [count changed, tool added](../../deltas/2026-08-20/f0bc295a8caaf4fbfad9.json): `1 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://aux.prdictionedge.ai/mcp/v1"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
