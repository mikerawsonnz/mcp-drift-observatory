# thirdhemisphere.agency: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/thirdhemisphere.agency.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://thirdhemisphere.agency/mcp` | 12 | [`2f8a26e0ef45`](b750b5af8da6e753c90e.json) | 2026-11-14 |

## Tools at `https://thirdhemisphere.agency/mcp`

- `get_blueprint_item_evidence`: `The data behind one play or move: your own numbers from the Blueprint, why it works and the research it rests on, and what not to do. DIY B…`
- `get_blueprint_progress`: `Where every play and move in your Blueprint stands, with the counts done, in progress, and not started. DIY Blueprint tool: needs a key who…`
- `get_company_authority_score`: `A company's published CRISP™ score and AI visibility reading in each market the AI Authority Index™ measures it in, with the month measured…`
- `get_company_score_history`: `Every dated reading the AI Authority Index™ has published for a company, oldest first: its rows in each edition and each market's Standing…`
- `get_edition_results`: `The published results of one AI Authority Index™ edition section: each company's Star Chart cell, CRISP™ score where it has one, the five f…`
- `get_market_standing`: `The companies in one market with a Standing Report, most named in AI answers first. Read-only. Every result carries its citation and link.`
- `get_my_blueprint_plan`: `Your Blueprint's ranked strategy plays and 90-day moves, each with an item_id, what to do, when, and how the next Blueprint measures it, wi…`
- `list_index_editions`: `Every published edition of Third Hemisphere's AI Authority Index™, with its markets (sections), publication date, DOI where recorded, and l…`
- `list_markets`: `Every market the AI Authority Index™ measures, with how many Standing Reports it has and when it was last measured. Read-only. Every result…`
- `list_my_blueprints`: `The AI Authority Blueprints sent to the address this key belongs to. Needs a key on a plan that includes DIY Blueprint tools. DIY Blueprint…`
- `search_companies`: `Find companies with a Standing Report in Third Hemisphere's AI Authority Index™ by name. Read-only. Every result carries its citation and l…`
- `update_blueprint_progress`: `Record where a play or move stands: not_started, in_progress, done, skipped, with an optional note of what was done. DIY Blueprint tool: ne…`

## Changes

- 2026-11-14: [description changed](../../deltas/2026-11-14/b750b5af8da6e753c90e.json): `6 field(s) changed`
- 2026-11-12: [field changed](../../deltas/2026-11-12/b750b5af8da6e753c90e.json): `1 field(s) changed`
- 2026-11-04: [count changed, tool added](../../deltas/2026-11-04/b750b5af8da6e753c90e.json): `5 tool(s) added; signals: url_introduced`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://thirdhemisphere.agency/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
