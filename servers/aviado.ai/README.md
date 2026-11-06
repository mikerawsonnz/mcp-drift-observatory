# aviado.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/aviado.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://aviado.ai/api/mcp` | 11 | [`94fec372ee2c`](112d81952274218832ad.json) | 2026-10-25 |

## Tools at `https://aviado.ai/api/mcp`

- `build_starter_stack`: `Starter stack (default 3, max 5) of recommendable supplements for a goal (e.g. 'insomnia', 'LDL cholesterol'), best-replicated app-visible…`
- `check_interaction`: `Point check of one pair, about 1-3 KB: a and b are each a supplement (name or canonical_id) or a medication (generic name; salt forms merge…`
- `get_biomarkers_for_supplement`: `Biomarkers a supplement moves in the Aviado app's evidence graph, one entry per biomarker (strongest edge), ordered by prior_weight (graph…`
- `get_interventions_for_biomarker`: `All mixed interventions in Aviado's evidence graph that move a biomarker, each labelled with intervention_type: supplement, food_substance,…`
- `get_supplement_info`: `Overview of one supplement: description, typical uses, its top 5 biomarkers (with up to 3 PubMed citations each), goals, mechanism tags and…`
- `get_supplement_interactions`: `Drug interactions come only from FDA drug labels and supplement-supplement ones only from Aviado's verified pairs; an empty result is not e…`
- `get_supplements_for_biomarker`: `Supplements in Aviado's evidence graph that move a biomarker (e.g. 'LDL cholesterol', 'HbA1c'). Lists only registry-classified supplements:…`
- `get_supplements_for_condition`: `Supplements associated with a health condition or goal (e.g. 'insomnia', 'anxiety', 'joint pain'), strongest evidence first. evidence_basis…`
- `get_top_brands`: `Highest-quality brands for a supplement: one product per brand (its best), ranked by ProofMark, Aviado's product quality score (testing, in…`
- `search_conditions`: `Find the condition id for a health condition, symptom or goal. Answers when the name matches one condition clearly (data.conditions lists i…`
- `search_supplements`: `Find the Aviado id for a supplement name, exactly (no fuzzy matching). Answers with matches[0] = the identity: vocabulary_exact, or user_in…`

## Changes

- 2026-10-25: [description changed](../../deltas/2026-10-25/112d81952274218832ad.json): `2 field(s) changed`
- 2026-10-16: [annotation changed, description changed, schema changed](../../deltas/2026-10-16/112d81952274218832ad.json): `10 field(s) changed; signals: length_more_than_doubled`
- 2026-10-14: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-10-14/112d81952274218832ad.json): `2 tool(s) added; 90 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://aviado.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
