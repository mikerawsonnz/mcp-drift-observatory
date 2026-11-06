# partsgraph.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/partsgraph.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://partsgraph.ai/api/mcp` | 11 | [`78567f5bb425`](0d667139b02888fec516.json) | 2026-08-20 |

## Tools at `https://partsgraph.ai/api/mcp`

- `build_bom`: `Composes a complete BOM for a reference build — quantities, dated indicative prices, per-line rationale, a compatibility verdict for the ch…`
- `check_compatibility`: `Evaluates a part set against the build's engineering constraints — supply windows, stall vs peak current, shaft/wheel fit, interfaces, sola…`
- `compare_parts`: `Aligned attribute-by-attribute comparison of two catalogue parts. Absence means the sources did not state a value — never that the part lac…`
- `fetch`: `Fetch the full provenance-backed record for a search result id as a citable document. Alias of get_part shaped to the search/fetch connecto…`
- `get_part`: `The complete canonical record for one part: every attribute with its provenance (source, page, verbatim quote, file hash), vendors with dat…`
- `get_provenance`: `The receipt behind a stated value: the verbatim source quote, the page, the extraction method, and the sha-256 of the exact file it was rea…`
- `list_builds`: `The catalogue's reference builds (robot, weather station, plant waterer) with their roles and candidate parts — the starting point for buil…`
- `list_categories`: `Every category in the catalogue with its part count.`
- `search`: `Search the Partsgraph demo catalogue. Returns result ids for fetch. Alias of search_parts shaped to the search/fetch connector contract.`
- `search_parts`: `Full-text search over the demo catalogue's provenance-backed part records. Filter by category, build or role. Every attribute returned was…`
- `view_bom`: `Composes the BOM for a reference build and renders it as an interactive view in clients that support MCP Apps. Same data as build_bom.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://partsgraph.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
