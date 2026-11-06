# mcp.flyvolo.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.flyvolo.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.flyvolo.ai/mcp` | 18 | [`705d33fdcd99`](70ce4e9834da1b9f696b.json) | 2026-09-26 |

## Tools at `https://mcp.flyvolo.ai/mcp`

- `describe_coverage`: `What VOLO covers and what it does not, including which occupations have no evidence yet. Call this when someone asks whether their job is c…`
- `find_affected`: `Which occupation and which specific tasks a change record bears on.`
- `find_evidence`: `Verified evidence records for an occupation, optionally for one task. Each record carries its scope (where it applies), its stage, whether…`
- `find_majors_for_occupation`: `Which degrees lead into this occupation.`
- `find_notes`: `VOLO's long-form answers to the big questions — how many jobs AI has actually taken, what actually gets automated, how long someone has, wh…`
- `find_notes_for_occupation`: `Which notes argue from this occupation's own records or task judgements. Use it to point someone from their own page to the wider answer.`
- `find_transition_paths`: `Options for someone in this occupation. Every path carries its real constraints (time, pay cut, seniority) and one action they can take thi…`
- `get_change`: `One verified change record by id, with VOLO's reading: what it means, what it does not yet establish, and what a reader can verify themselv…`
- `get_change_history`: `The verified change timeline for an occupation, oldest first.`
- `get_major`: `A degree and the occupations it feeds. There is no score for a major and never will be — answer 'should I switch majors' by pointing at whe…`
- `get_note`: `The full text of one note, section by section, each section with the verified records it rests on. Use it when you need to quote or cite ra…`
- `get_occupation`: `Full task-level assessment of one occupation. Every task carries direction, basis (evidenced vs inferred) and limits — what that judgement…`
- `get_ontology`: `Where an occupation or a degree sits in the official classifications (U.S. Department of Labor O*NET 31.0; U.S. Department of Education CIP…`
- `get_role_tasks`: `The task breakdown for one occupation. The unit of assessment is the task, never the job title.`
- `list_business_functions`: `For the business side: the functions a company is organised into, and which occupations sit in each. Use this when someone describes a comp…`
- `query_ontology`: `Walk the VOLO Ontology directly. No arguments: the object types and link types. 'type': the objects of that type. 'type' + 'id': one object…`
- `resolve_occupation_or_major`: `Resolve a job title, a company's internal name for a role, a nickname or a degree name to a canonical VOLO entity. Call this FIRST whenever…`
- `search`: `Search occupations, majors and verified change records by keyword. Returns entries, not judgements.`

## Changes

- 2026-09-26: [count changed, tool added](../../deltas/2026-09-26/70ce4e9834da1b9f696b.json): `2 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.flyvolo.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
