# solar.agentlookups.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/solar.agentlookups.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://solar.agentlookups.ai/mcp` | 2 | [`fd07d22d2d81`](5f9bb98ffa45d7ea20ff.json) | 2026-09-29 |

## Tools at `https://solar.agentlookups.ai/mcp`

- `solar_law`: `Returns the full GreenLight registry record for one state's plug-in (balcony) solar law: legal status, the law's name and dates, key provis…`
- `solar_states`: `Lists every state in the GreenLight plug-in (balcony) solar registry with its legal status, law name, power cap, and verification state, pl…`

## Changes

- 2026-09-29: [description changed, field changed, schema changed](../../deltas/2026-09-29/5f9bb98ffa45d7ea20ff.json): `5 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://solar.agentlookups.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
