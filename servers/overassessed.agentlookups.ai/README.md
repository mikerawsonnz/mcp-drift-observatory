# overassessed.agentlookups.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/overassessed.agentlookups.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://overassessed.agentlookups.ai/mcp` | 1 | [`af24b4cfaff8`](c6dae6909013339ef565.json) | 2026-10-28 |

## Tools at `https://overassessed.agentlookups.ai/mcp`

- `check_assessment`: `Fairness check for one Maryland property assessment against genuinely similar homes (same triennial reassessment group, similar size, lot a…`

## Changes

- 2026-10-28: [description changed, schema changed](../../deltas/2026-10-28/c6dae6909013339ef565.json): `3 field(s) changed`
- 2026-10-27: [description changed, schema changed](../../deltas/2026-10-27/c6dae6909013339ef565.json): `4 field(s) changed; signals: length_more_than_doubled`
- 2026-09-30: [description changed](../../deltas/2026-09-30/c6dae6909013339ef565.json): `1 field(s) changed`
- 2026-09-29: [description changed, field changed, schema changed](../../deltas/2026-09-29/c6dae6909013339ef565.json): `5 field(s) changed; signals: length_more_than_doubled`
- 2026-09-28: [annotation changed](../../deltas/2026-09-28/c6dae6909013339ef565.json): `5 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://overassessed.agentlookups.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
