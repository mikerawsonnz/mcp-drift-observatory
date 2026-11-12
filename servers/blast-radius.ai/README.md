# blast-radius.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/blast-radius.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://blast-radius.ai/mcp` | 9 | [`1e58b048aac0`](6e0fc9f43e7d724c3c48.json) | 2026-11-12 |

## Tools at `https://blast-radius.ai/mcp`

- `ask_blast_radius`: `Ask a question about the Blast Radius brief and its recent news. Retrieval is semantic (embedding similarity): returns the closest memo sec…`
- `assess_against_frontier_line`: `Stress-test a company, product, or thesis against the Blast Radius 'Frontier Line' framework, an adversarial business-model survivability a…`
- `get_diligence_checklist`: `Get the structured Blast Radius diligence checklist: the key anti-patterns and durable-startup characteristics used to assess AI-first comp…`
- `get_force_reading`: `Get one force's current weekly reading (with its week, direction, paragraphs, and cited story pages), up to ten of its latest events, the m…`
- `get_igv_quote`: `Get the current IGV (iShares Expanded Tech-Software ETF) quote, the SaaSpocalypse market signal referenced in the brief.`
- `get_latest_update`: `Get this week's lede and the five force readings: the latest published weekly readings of the Blast Radius argument, each linked to the sto…`
- `get_thesis`: `Get the durable Blast Radius thesis and key metrics, plus the current IGV software-ETF quote.`
- `get_top_headlines`: `Get the last seven days of ranked Blast Radius news: the Top Headlines strip in order and up to five leading events per force, each with it…`
- `subscribe`: `Request an email-confirmation link for Blast Radius updates-only signup. The reader must confirm before activation.`

## Changes

- 2026-11-12: [description changed](../../deltas/2026-11-12/6e0fc9f43e7d724c3c48.json): `1 field(s) changed`
- 2026-11-07: [description changed](../../deltas/2026-11-07/6e0fc9f43e7d724c3c48.json): `1 field(s) changed`
- 2026-09-27: [count changed, description changed, tool added](../../deltas/2026-09-27/6e0fc9f43e7d724c3c48.json): `2 tool(s) added; 4 field(s) changed`
- 2026-09-10: [description changed](../../deltas/2026-09-10/6e0fc9f43e7d724c3c48.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://blast-radius.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
