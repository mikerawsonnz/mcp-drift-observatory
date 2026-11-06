# hyperscale0.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/hyperscale0.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://hyperscale0.ai/v1/mcp` | 2 | [`4cf93478d266`](f53ed514de1fbd668e59.json) | 2026-09-18 |

## Tools at `https://hyperscale0.ai/v1/mcp`

- `extension_list`: `List catalog extensions.`
- `kyc_requirements_retrieve`: `Retrieve KYC tier requirements.`

## Changes

- 2026-09-18: [count changed, description changed, schema changed, tool added](../../deltas/2026-09-18/f53ed514de1fbd668e59.json): `1 tool(s) added; 162 field(s) changed; signals: url_introduced`
- 2026-09-15: [count changed, description changed, tool removed](../../deltas/2026-09-15/f53ed514de1fbd668e59.json): `2 tool(s) removed; 1 field(s) changed`
- 2026-09-12: [description changed](../../deltas/2026-09-12/f53ed514de1fbd668e59.json): `3 field(s) changed`
- 2026-09-11: [schema changed](../../deltas/2026-09-11/f53ed514de1fbd668e59.json): `58 field(s) changed; signals: length_more_than_doubled`
- 2026-09-10: [schema changed](../../deltas/2026-09-10/f53ed514de1fbd668e59.json): `1359 field(s) changed`
- 2026-09-05: [schema changed](../../deltas/2026-09-05/f53ed514de1fbd668e59.json): `42 field(s) changed`
- 2026-09-04: [field changed, schema changed](../../deltas/2026-09-04/f53ed514de1fbd668e59.json): `36 field(s) changed; signals: length_more_than_doubled`
- 2026-09-01: [description changed, schema changed](../../deltas/2026-09-01/f53ed514de1fbd668e59.json): `373 field(s) changed; signals: length_more_than_doubled`
- 2026-08-31: [count changed, description changed, schema changed, tool removed](../../deltas/2026-08-31/f53ed514de1fbd668e59.json): `47 tool(s) removed; 337 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://hyperscale0.ai/v1/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
