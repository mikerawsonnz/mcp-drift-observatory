# api.askmiles.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.askmiles.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.askmiles.ai/mcp` | 5 | [`df5685820fdd`](1102b75e3d77ee7a2424.json) | 2026-10-17 |

## Tools at `https://api.askmiles.ai/mcp`

- `compare_card_facts`: `The same catalog record for 2-5 cards at once, for comparing fees, networks and which benefits each carries. Card facts only — no earning r…`
- `estimate_point_value`: `Miles' own estimate of a loyalty point's value in cents, optionally multiplied by a balance. Call with no arguments to list every program M…`
- `find_transfer_routes`: `Which loyalty programs a currency transfers to, or which currencies reach a destination, and whether a transfer bonus is running. This is t…`
- `get_card_facts`: `Everything the public catalog holds on one card: issuer, annual fee, network, foreign transaction fee, rewards currency, and the names of i…`
- `search_card_catalog`: `Find credit cards open to new applicants by issuer, annual fee, network, rewards currency, or a benefit they carry. Returns a short row per…`

## Changes

- 2026-10-17: [schema changed](../../deltas/2026-10-17/1102b75e3d77ee7a2424.json): `1 field(s) changed`
- 2026-09-30: [schema changed](../../deltas/2026-09-30/1102b75e3d77ee7a2424.json): `9 field(s) changed; signals: length_more_than_doubled`
- 2026-09-24: [schema changed](../../deltas/2026-09-24/1102b75e3d77ee7a2424.json): `3 field(s) changed; signals: length_more_than_doubled`
- 2026-08-31: [schema changed](../../deltas/2026-08-31/1102b75e3d77ee7a2424.json): `16 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.askmiles.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
