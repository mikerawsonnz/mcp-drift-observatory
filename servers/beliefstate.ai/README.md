# beliefstate.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/beliefstate.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://beliefstate.ai/v1/research/mcp` | 18 | [`fa52f4e1b356`](d29176e06366706dabab.json) | 2026-11-06 |

## Tools at `https://beliefstate.ai/v1/research/mcp`

- `compare_beliefs`: `Compare two cited investment cases for support, contradiction or dependency, including explicit unknown and unrelated outcomes. Optional co…`
- `evaluate_belief_scenario`: `Apply up to eight hypothetical condition assumptions to a case's recorded scenario model. Does not alter evidence or predict the investor's…`
- `get_author_track_record`: `Read an investor's stored publication-based outcome cohorts over one explicit ticker, entity, Belief or released corpus scope and optional…`
- `get_belief`: `Read a requested complete investment case or evidence beyond a brief, with risks, conditions and coverage gaps. An ordinary library overvie…`
- `get_belief_catalysts`: `Read evidence-linked Catalyst objects with qualified current status or explicit unknowns. Filter one ticker, entity, Belief or released cor…`
- `get_belief_changes`: `Read a mixed, ordered change journal: author-view revisions, distribution changes and calculated publication outcomes are separate domains…`
- `get_belief_relationships`: `Inspect cited relationship paths within one investment case. Preserves stated links, engine inferences and unknowns. Per-call x402 price: 0…`
- `get_belief_risks`: `Read evidence-linked Risk objects for exactly one ticker, entity, Belief or explicit released corpus. Filter by person, source, publication…`
- `get_beliefs`: `List dated investment ideas for a requested inventory or filtered research on one ticker or subject. Investor, direction and time filters a…`
- `get_brief`: `Start with overview for an ordinary company or ETF research question, including outlook and changes. Present findings in plain language wit…`
- `get_context_assessment`: `Open a dated engine context assessment and its permitted evidence. Engine analysis is separate from an investor's stated view. Per-call x40…`
- `get_research_visual`: `Read one cited chart or table, including its regions and paginated exact rows or data points. Per-call x402 price: 0.02 USDC on Base.`
- `get_tickers`: `Free research coverage and company discovery.`
- `list_research_visuals`: `List cited charts and tables for one investment case or context assessment. Per-call x402 price: 0.02 USDC on Base.`
- `refresh_market_data`: `Explicitly refresh missing or stale market data for one current company or subject, then return its research brief. Per-call x402 price: 0.…`
- `search_beliefs`: `Find investment ideas by thesis, topic or trade setup, with cited matching passages. Per-call x402 price: 1.50 USDC on Base.`
- `search_companies`: `Free research coverage and company discovery.`
- `search_entities`: `Find released companies, industries, themes and other research subjects by name or kind. Per-call x402 price: 0.02 USDC on Base.`

## Changes

- 2026-11-06: [schema changed](../../deltas/2026-11-06/d29176e06366706dabab.json): `31954 field(s) changed; signals: length_more_than_doubled`
- 2026-11-05: [schema changed](../../deltas/2026-11-05/d29176e06366706dabab.json): `25644 field(s) changed; signals: length_more_than_doubled`
- 2026-11-04: [schema changed](../../deltas/2026-11-04/d29176e06366706dabab.json): `37864 field(s) changed; signals: length_more_than_doubled`
- 2026-11-03: [schema changed](../../deltas/2026-11-03/d29176e06366706dabab.json): `1 field(s) changed`
- 2026-11-02: [schema changed](../../deltas/2026-11-02/d29176e06366706dabab.json): `39227 field(s) changed; signals: length_more_than_doubled`
- 2026-11-01: [schema changed](../../deltas/2026-11-01/d29176e06366706dabab.json): `41414 field(s) changed`
- 2026-10-31: [schema changed](../../deltas/2026-10-31/d29176e06366706dabab.json): `36949 field(s) changed; signals: length_more_than_doubled`
- 2026-10-29: [description changed, schema changed](../../deltas/2026-10-29/d29176e06366706dabab.json): `16 field(s) changed`
- 2026-10-28: [description changed, schema changed](../../deltas/2026-10-28/d29176e06366706dabab.json): `40618 field(s) changed; signals: length_more_than_doubled`
- 2026-10-27: [count changed, tool added](../../deltas/2026-10-27/d29176e06366706dabab.json): `16 tool(s) added`
- 2026-10-26: [count changed, tool removed](../../deltas/2026-10-26/d29176e06366706dabab.json): `16 tool(s) removed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://beliefstate.ai/v1/research/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
