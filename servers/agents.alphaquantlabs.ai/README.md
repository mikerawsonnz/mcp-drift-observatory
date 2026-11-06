# agents.alphaquantlabs.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agents.alphaquantlabs.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agents.alphaquantlabs.ai/v1/mcp` | 2 | [`a643363e9a6b`](c307148b3e77d7c2db4d.json) | 2026-10-25 |

## Tools at `https://agents.alphaquantlabs.ai/v1/mcp`

- `check_address`: `FREE, no key. Use when you have one specific street address in the City of Gold Coast or Brisbane City (Queensland, Australia) and need to…`
- `get_full_report`: `Full structured PropertyCheck JSON (propertycheck/2) for one covered address: identity, coverage, capabilities, a summary and up to twelve…`

## Changes

- 2026-10-25: [description changed, schema changed](../../deltas/2026-10-25/c307148b3e77d7c2db4d.json): `4 field(s) changed`
- 2026-10-14: [description changed](../../deltas/2026-10-14/c307148b3e77d7c2db4d.json): `2 field(s) changed`
- 2026-10-13: [description changed, schema changed](../../deltas/2026-10-13/c307148b3e77d7c2db4d.json): `11 field(s) changed`
- 2026-10-11: [count changed, tool added, tool removed](../../deltas/2026-10-11/c307148b3e77d7c2db4d.json): `2 tool(s) added; 10 tool(s) removed; signals: imperative_language_introduced` **(notable)**
- 2026-10-10: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-10-10/c307148b3e77d7c2db4d.json): `7 field(s) changed`
- 2026-10-08: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-08/c307148b3e77d7c2db4d.json): `1 tool(s) added; 23 field(s) changed`
- 2026-10-06: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-06/c307148b3e77d7c2db4d.json): `2 tool(s) added; 3 field(s) changed`
- 2026-10-03: [count changed, description changed, tool added](../../deltas/2026-10-03/c307148b3e77d7c2db4d.json): `1 tool(s) added; 1 field(s) changed`
- 2026-10-02: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-10-02/c307148b3e77d7c2db4d.json): `18 field(s) changed`
- 2026-10-01: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-10-01/c307148b3e77d7c2db4d.json): `23 field(s) changed; signals: length_more_than_doubled`
- 2026-09-30: [description changed, schema changed](../../deltas/2026-09-30/c307148b3e77d7c2db4d.json): `7 field(s) changed; signals: length_more_than_doubled`
- 2026-09-29: [annotation changed, count changed, description changed, tool added](../../deltas/2026-09-29/c307148b3e77d7c2db4d.json): `3 tool(s) added; 2 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agents.alphaquantlabs.ai/v1/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
