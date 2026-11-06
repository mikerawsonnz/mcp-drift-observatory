# pocketdrives.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/pocketdrives.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://pocketdrives.ai/mcp` | 9 | [`1f3f73ab9c6e`](5ca848d3f0b79cf460e3.json) | 2026-08-20 |

## Tools at `https://pocketdrives.ai/mcp`

- `drives_airport_search`: `Search airports for delivery pickup with delivery fee information.`
- `drives_get_quote`: `Calculate a full rental quote including daily breakdown, taxes, deposit, and total for a date range.`
- `drives_host_showroom`: `Get a host profile page with bio, locations, team, and social links by username.`
- `drives_location_suggest`: `Autocomplete cities, airports, and venues for search location input.`
- `drives_search_vehicles`: `Search the Pocket Drives marketplace for available rental vehicles by location, dates, category, and filters.`
- `drives_vehicle_availability`: `Get a monthly availability calendar with daily rates for a vehicle.`
- `drives_vehicle_detail`: `Get full details for a specific vehicle including rates, host info, and organization policies.`
- `drives_vehicle_reviews`: `List published renter reviews for a vehicle. Uses asset_id (not asset_rental_id) per the GraphQL schema.`
- `drives_venue_search`: `Search stadiums, arenas, and venues for delivery pickup with delivery fee information.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://pocketdrives.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
