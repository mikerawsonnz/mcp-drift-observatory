# droneintelligence.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/droneintelligence.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://droneintelligence.ai/api/mcp` | 12 | [`67c0949dfe38`](21600b2320877eb99492.json) | 2026-08-20 |

## Tools at `https://droneintelligence.ai/api/mcp`

- `compare_companies`: `A Drone Intelligence side-by-side company comparison by slug, e.g. droneshield-vs-dedrone.`
- `get_briefing`: `Full text of a Drone Intelligence Signal Dossier briefing by slug: executive summary, signals, assessment, sources.`
- `get_company_profile`: `A Drone Intelligence company profile by slug: positioning, sourced facts, funding, contracts, products.`
- `get_intelligence_page`: `A Drone Intelligence market intelligence page by slug: overview, sections, key players, outlook, sources.`
- `get_products`: `The commercial products, machine-readable: what they are, prices, checkout URLs, licence terms.`
- `list_catalogue`: `Paginated slugs of Drone Intelligence content by type (briefing, intelligence, company, comparison). 50 per page.`
- `search_content`: `Search Drone Intelligence briefings, market intelligence pages, company profiles and comparisons. Returns up to 10 matches with title, type…`
- `tracker_aggregate`: `Counts of tracker awards grouped by theatre, layer, or awardee. Requires a tracker licence token.`
- `tracker_awards`: `Query the 76 sourced counter-UAS awards. Filter by theatre, kill-chain layer, or awardee substring. Requires a tracker licence token.`
- `tracker_capital_ledger`: `The tracker's capital and acquisition ledger: where the money behind the counter-UAS vendors is being raised. Requires a tracker licence to…`
- `tracker_schema`: `Metadata for the paid Counter-UAS Tracker dataset: fields, theatres, layers, counts, data-through date, licence. Requires a tracker licence…`
- `tracker_vendor_matrix`: `Query the 45-vendor counter-UAS competitive matrix. Filter by layer or US-procurement eligibility. Requires a tracker licence token.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://droneintelligence.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
