# state.1court.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/state.1court.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://state.1court.ai/api/mcp` | 6 | [`53bc354086e3`](c36a3ccafbf96b7eca38.json) | 2026-11-04 |

## Tools at `https://state.1court.ai/api/mcp`

- `calculate_deadline`: `Calculate a court deadline deterministically from cited rules (weekends, legal holidays, short-period and mail-service rules applied). Retu…`
- `get_court_info`: `Get verified court information for a specific U.S. county: clerk of court contacts, e-filing provider and whether e-filing is mandatory, fi…`
- `list_counties`: `List the counties covered in a given U.S. state (accepts a full state name, 2-letter code, or slug). Returns each county name and its 1Cour…`
- `list_deadline_rules`: `List the court deadline types 1Court can calculate for a jurisdiction. Available ids: TX; CA (civil), CA-FAM (family), CA-PROB (probate), C…`
- `list_states`: `List all U.S. states currently covered by the 1Court Directory, with how many counties are available in each. Use this to discover coverage…`
- `search_courts`: `Search the 1Court Directory by county or state name and get matching counties with their 1Court page URLs. Use when you are unsure of the e…`

## Changes

- 2026-11-04: [description changed, schema changed](../../deltas/2026-11-04/c36a3ccafbf96b7eca38.json): `3 field(s) changed`
- 2026-10-29: [description changed, schema changed](../../deltas/2026-10-29/c36a3ccafbf96b7eca38.json): `3 field(s) changed`
- 2026-10-28: [description changed, schema changed](../../deltas/2026-10-28/c36a3ccafbf96b7eca38.json): `3 field(s) changed`
- 2026-10-27: [description changed, schema changed](../../deltas/2026-10-27/c36a3ccafbf96b7eca38.json): `5 field(s) changed`
- 2026-10-25: [description changed, schema changed](../../deltas/2026-10-25/c36a3ccafbf96b7eca38.json): `11 field(s) changed`
- 2026-10-24: [count changed, tool added](../../deltas/2026-10-24/c36a3ccafbf96b7eca38.json): `2 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://state.1court.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
