# cold-api.coldstate.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/cold-api.coldstate.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://cold-api.coldstate.ai/mcp` | 16 | [`718230c857a9`](2253bdfad81275d9ddd2.json) | 2026-10-01 |

## Tools at `https://cold-api.coldstate.ai/mcp`

- `coldstate_batch_search`: `Run several knowledge-base queries in one call against a single consistent kb_snapshot. Returns each query with its ranked results — effici…`
- `coldstate_browse_documents`: `Browse documents in a ColdState index. Indexes are zero-knowledge, so each document is returned as your ref_id plus its state classificatio…`
- `coldstate_capabilities`: `Machine-readable manifest of this server: available tools, knowledge domains, current kb_snapshot, determinism guarantees, and limits. Call…`
- `coldstate_cite`: `Get a canonical, reproducible citation for a knowledge entry by id (title, domain, source, content_hash, kb_snapshot). Cite a fact so it ca…`
- `coldstate_domains`: `List all available knowledge domains in ColdState's global knowledge base with entry counts.`
- `coldstate_explain`: `Explain why a specific document ranked for a query. Returns a per-term relevance breakdown and an overall match summary — deterministic and…`
- `coldstate_fetch`: `Fetch a single knowledge-base entry verbatim by its stable id (e.g. "eng_000229f438f7cebd"). Deterministic retrieval — returns the full rec…`
- `coldstate_isomorph`: `Cross-domain structural analog: given a knowledge entry id, find its closest structural twin in each OTHER domain ("same structure, differe…`
- `coldstate_list_indexes`: `List all your ColdState indexes with their status, mode, document count, and domain preset.`
- `coldstate_related`: `Find knowledge entries deterministically related to a given entry id via ColdState's concept-cluster graph. Returns same-cluster and neighb…`
- `coldstate_resolve`: `Resolve a name, alias, or surface form to its canonical ColdState knowledge entry (id + title). Deterministic: an exact title match wins, e…`
- `coldstate_search`: `Search a ColdState index by collection name or index ID. Returns ranked results with Ψ scores and state classification (CRYSTALLINE/FLUID/R…`
- `coldstate_search_global`: `Search ColdState's global knowledge base (48.4M+ entries across 35 domains including SCIENCE, MEDICINE, TECHNOLOGY, HISTORY, etc). Returns…`
- `coldstate_snapshot`: `Get the current knowledge-base snapshot/version id. Pin this kb_snapshot for reproducibility: the same query against the same kb_snapshot r…`
- `coldstate_stats`: `Deterministic statistics. With a 'query': total matches + state distribution of the top results. Without: global knowledge-base stats (entr…`
- `coldstate_verify`: `Verify a previously-cited knowledge fact is unchanged. Provide the entry id and the content_hash you stored earlier; returns whether it sti…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://cold-api.coldstate.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
