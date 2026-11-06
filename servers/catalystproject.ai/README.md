# catalystproject.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/catalystproject.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://catalystproject.ai/mcp` | 7 | [`082c200b01dc`](3ee907b964adff5cc9f7.json) | 2026-11-06 |

## Tools at `https://catalystproject.ai/mcp`

- `find_evidence`: `Answers "what does X do?" and "does X affect Y?" for a supplement, nutrient, drug, food compound or plant (for example "does magnesium help…`
- `get_finding`: `Explains one finding by its finding id: the claim, its evidence strength and what that level means, the verbatim quote, the study design an…`
- `get_findings`: `Lists the curated study findings for one node by id, from search_nodes: for a compound, organism or material, what it has been shown to aff…`
- `get_reactions`: `Lists the biochemical reactions from Rhea and Human-GEM that a compound is a substrate or product of, or that a protein (enzyme) catalyses…`
- `get_relations`: `Lists what public reference databases (Reactome, UniProt, Rhea, ChEBI and others) record about one node by id, from search_nodes: transport…`
- `reach`: `Answers a route question: "can X become Y in the body" (give from_id and to_id) and "what can X become" (give only from_id). Both ids are c…`
- `search_nodes`: `Looks up the node id for a compound, protein, organism or outcome by name or synonym (for example "CoQ10", "caffeine", "CYP1A2", "sleep").…`

## Changes

- 2026-11-06: [description changed, schema changed](../../deltas/2026-11-06/3ee907b964adff5cc9f7.json): `68 field(s) changed; signals: length_more_than_doubled`
- 2026-11-05: [description changed](../../deltas/2026-11-05/3ee907b964adff5cc9f7.json): `3 field(s) changed`
- 2026-11-03: [description changed, field changed](../../deltas/2026-11-03/3ee907b964adff5cc9f7.json): `9 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://catalystproject.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
