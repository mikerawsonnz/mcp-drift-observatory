# rx.agentlookups.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/rx.agentlookups.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://rx.agentlookups.ai/mcp` | 1 | [`a0a911c1e92e`](dd2c3869e34da13c6fa0.json) | 2026-10-28 |

## Tools at `https://rx.agentlookups.ai/mcp`

- `drug_price`: `Looks up what US pharmacies actually pay to acquire a drug (the CMS NADAC benchmark, per unit, with its date; for a pen, syringe, autoinjec…`

## Changes

- 2026-10-28: [description changed](../../deltas/2026-10-28/dd2c3869e34da13c6fa0.json): `1 field(s) changed`
- 2026-10-27: [description changed](../../deltas/2026-10-27/dd2c3869e34da13c6fa0.json): `1 field(s) changed`
- 2026-10-13: [description changed](../../deltas/2026-10-13/dd2c3869e34da13c6fa0.json): `1 field(s) changed`
- 2026-10-10: [description changed](../../deltas/2026-10-10/dd2c3869e34da13c6fa0.json): `1 field(s) changed`
- 2026-09-30: [description changed](../../deltas/2026-09-30/dd2c3869e34da13c6fa0.json): `1 field(s) changed; signals: length_more_than_doubled`
- 2026-09-29: [description changed, field changed](../../deltas/2026-09-29/dd2c3869e34da13c6fa0.json): `2 field(s) changed; signals: length_more_than_doubled`
- 2026-09-28: [annotation changed](../../deltas/2026-09-28/dd2c3869e34da13c6fa0.json): `5 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://rx.agentlookups.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
