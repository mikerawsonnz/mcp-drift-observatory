# fenlight.waggle.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/fenlight.waggle.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://fenlight.waggle.ae/mcp` | 8 | [`129974ab4107`](080eb55643f26382f415.json) | 2026-10-24 |

## Tools at `https://fenlight.waggle.ae/mcp`

- `ai_answers`: `Put a buyer's question to an AI assistant that searches the live web, and see whether a brand and its competitors are named in the answer,…`
- `company_serp_footprint`: `Audit a company's SERP digital footprint, brand reputation, owned domains, and entity profiles. Separates owned web properties, social/enti…`
- `extract_local_places`: `Extract Google Local Pack (3-pack) and Google Places listings for local queries. Returns place_id/cid, title, rating, review count, address…`
- `extract_shopping_results`: `Extract Google Shopping carousel listings for e-commerce and product queries. Returns product title, price, currency, merchant, rating, rev…`
- `find_discussion_candidates`: `Search Google and filter organic results (positions 1-100) specifically for community discussions and forum threads (Reddit, Quora, HackerN…`
- `geo_citation_radar`: `Run GEO Citation & Injection Radar for a topic query and brand. Calculates citation probability score (0-100), identifies high-impact Reddi…`
- `google_serp`: `Execute a full Google SERP search query with strict Google provenance (depth 10 to 100). Returns verified Google organic results with class…`
- `keyword_ideas`: `Keyword ideas for a seed keyword from Google autocomplete (the seed plus question words or the alphabet), People Also Ask and related searc…`

## Changes

- 2026-10-24: [description changed](../../deltas/2026-10-24/080eb55643f26382f415.json): `2 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://fenlight.waggle.ae/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
