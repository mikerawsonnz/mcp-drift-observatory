# state.1court.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/state.1court.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://state.1court.ai/api/mcp` | 9 | [`763ac4ca9f0e`](c36a3ccafbf96b7eca38.json) | 2026-11-07 |

## Tools at `https://state.1court.ai/api/mcp`

- `calculate_deadline`: `Calculate a court deadline from cited rules (weekends, court holidays, service extensions and local rules applied). Returns the date, each…`
- `get_court_info`: `Get verified court information for one U.S. county: clerk contacts, courthouse address, e-filing provider and whether it is mandatory, fili…`
- `get_rule`: `Get one deadline rule: its period, trigger, citation, the verbatim rule text, the official source URL, the 1Court rule page, any disclosed…`
- `list_counties`: `List the counties covered in a U.S. state (full name, 2-letter code or slug), each with its 1Court page URL.`
- `list_deadline_rules`: `List the deadline types 1Court can calculate for one rule set (TX, CA, CA-FAM, CA-APP, US, US-BK, US-CRIM, CA-PROB, CA-UD, CA-SC, CA-GOV, C…`
- `list_rule_sets`: `List every deadline rule set 1Court covers, with rule counts and scope. Coverage: Deadlines: California in depth (civil, family, probate, e…`
- `list_states`: `List the U.S. states in the 1Court Directory, with how many counties each has. Use this to discover coverage before looking up a county.`
- `search_courts`: `Search the 1Court Directory by county or state name, courthouse name, city, or phone number. Returns matching counties and courthouses with…`
- `search_rules`: `Find deadline rules by plain words (for example "opposition to motion", "answer complaint", "notice of appeal"). Searches rule names, ids,…`

## Changes

- 2026-11-07: [annotation changed, count changed, description changed, schema changed, tool added](../../deltas/2026-11-07/c36a3ccafbf96b7eca38.json): `3 tool(s) added; 13 field(s) changed; signals: length_more_than_doubled`
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
