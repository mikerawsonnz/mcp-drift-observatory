# app.bezal.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.bezal.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.bezal.ai/api/mcp` | 9 | [`4b61485295fc`](4cca1c526a32cc31d3b0.json) | 2026-11-11 |

## Tools at `https://app.bezal.ai/api/mcp`

- `check_business_availability`: `Check whether a business is open on a date, based on its posted opening hours. Hours are shared only for providers on a paid Bezal plan, an…`
- `compare_businesses`: `Compare up to 5 businesses side by side: the public profile fields plus services, BezalRank and whether the profile is claimed. Every busin…`
- `get_business`: `Get the public Bezal profile for one business by UUID. Every business includes name, category, city, state, rating, review count, tier and…`
- `get_reviews`: `Get reviews for a specific business: Bezal reviews (rating, text, verified flag, date and the reviewer as first name and last initial) plus…`
- `get_service_catalog`: `Get services and pricing for a specific business. Falls back to the list of service names if no priced catalog exists.`
- `list_categories`: `List all available business categories in the directory.`
- `search_businesses`: `Search local business profiles on Bezal by name, category, or location. Every business includes name, category, city, state, rating, review…`
- `search_by_city`: `Search for businesses in a specific city, optionally filtered by category. Every business includes name, category, city, state, rating, rev…`
- `search_by_service`: `Find businesses that list a specific service, when you know the exact service rather than the category (for example "Drain cleaning" rather…`

## Changes

- 2026-11-11: [description changed](../../deltas/2026-11-11/4cca1c526a32cc31d3b0.json): `5 field(s) changed`
- 2026-11-08: [schema changed](../../deltas/2026-11-08/4cca1c526a32cc31d3b0.json): `1 field(s) changed`
- 2026-10-29: [annotation changed, count changed, description changed, field changed, tool removed](../../deltas/2026-10-29/4cca1c526a32cc31d3b0.json): `4 tool(s) removed; 32 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.bezal.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
