# env.agentlookups.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/env.agentlookups.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://env.agentlookups.ai/mcp` | 4 | [`ab0ae41f25c1`](e4737c6c08d0e753c7d6.json) | 2026-11-01 |

## Tools at `https://env.agentlookups.ai/mcp`

- `broadband_availability`: `Fixed broadband availability for a US location from the FCC Broadband Data Collection (BDC), counted per 2020 Census block: each provider a…`
- `drinking_water`: `Public water systems for a US location, from EPA's quarterly drinking-water data (SDWA; GroundTruth checks for a new quarter monthly), with…`
- `environment_near`: `Environmental records within a radius of a US location, from GroundTruth's monthly snapshot of three EPA datasets: National Priorities List…`
- `location_scores`: `Layer scores for a US location: school quality, natural hazards, groundwater contamination, Superfund proximity, air quality, highway noise…`

## Changes

- 2026-11-01: [description changed](../../deltas/2026-11-01/e4737c6c08d0e753c7d6.json): `1 field(s) changed`
- 2026-10-28: [description changed](../../deltas/2026-10-28/e4737c6c08d0e753c7d6.json): `3 field(s) changed`
- 2026-10-27: [annotation changed, description changed, schema changed](../../deltas/2026-10-27/e4737c6c08d0e753c7d6.json): `17 field(s) changed; signals: length_more_than_doubled, url_introduced`
- 2026-10-22: [description changed](../../deltas/2026-10-22/e4737c6c08d0e753c7d6.json): `1 field(s) changed`
- 2026-10-16: [description changed](../../deltas/2026-10-16/e4737c6c08d0e753c7d6.json): `1 field(s) changed`
- 2026-10-06: [description changed, tool added, tool removed](../../deltas/2026-10-06/e4737c6c08d0e753c7d6.json): `1 tool(s) added; 1 tool(s) removed; 1 field(s) changed`
- 2026-10-04: [count changed, tool added](../../deltas/2026-10-04/e4737c6c08d0e753c7d6.json): `1 tool(s) added`
- 2026-09-30: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-09-30/e4737c6c08d0e753c7d6.json): `31 field(s) changed; signals: length_more_than_doubled`
- 2026-08-29: [description changed](../../deltas/2026-08-29/e4737c6c08d0e753c7d6.json): `1 field(s) changed`
- 2026-08-27: [description changed](../../deltas/2026-08-27/e4737c6c08d0e753c7d6.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://env.agentlookups.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
