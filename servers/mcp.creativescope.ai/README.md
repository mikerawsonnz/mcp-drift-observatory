# mcp.creativescope.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.creativescope.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.creativescope.ai/mcp` | 35 | [`4f0b7c7da4b1`](611783010d7bc9a98efa.json) | 2026-09-10 |

## Tools at `https://mcp.creativescope.ai/mcp`

- `compare_games`: `Compare 2-5 games with the same date range, deduplication and metric definitions. Return creative, reused-creative and ad-plan counts plus…`
- `get_context`: `Get CreativeScope business context, current date, supported platforms, registered tool catalog, date limits, freshness and capability bound…`
- `get_filter_options`: `Get valid game categories, countries and 14 delivery-platform aliases. Map user conditions to the returned standard values before exact fil…`
- `get_game_ads_v2`: `Discover a game's ad plans by countries, platforms, format and dates. Deduplicate cross-month snapshots; each result represents one plan wi…`
- `get_game_country_distribution`: `Get game delivery-country coverage for a date range. Country coverage can overlap and does not represent country-specific exposure or audie…`
- `get_game_daily_impressions`: `Get daily and cumulative estimated exposure across all Android/iOS packages associated with a game. daily_impressions is the daily incremen…`
- `get_game_detail`: `Get game identity, delivery platforms, countries, active ad and creative counts, and download snapshots. Exposure for active creatives is l…`
- `get_game_install_trend`: `Get daily Google Play net download increments and cumulative snapshots for a game. Return requested and actual coverage dates, download_inc…`
- `get_game_investment_trend`: `Get daily newly launched creatives, reused creatives, ad plans and exposure references to analyze delivery growth and creative refresh cade…`
- `get_game_materials`: `List a game advertiser's creatives by delivery performance, including material_reference, delivery dates, heat, reuse status and media. No…`
- `get_game_overview`: `Get a game's identity, deduplicated creatives/ad plans, market and platform coverage, and delivery-cadence summary in one call. Require exp…`
- `get_game_platform_stats`: `Get deduplicated creative count, first-discovered creative count and ad-plan count for one game, platform and explicit date range (maximum…`
- `get_game_publisher_platform_ratio`: `Get a game delivery-platform distribution for a date range. Platform coverage can overlap; shares are not exclusive audience or exposure sh…`
- `get_game_publisher_platform_trend`: `Get a game delivery-platform trend for a date range. Use the returned metric and dates consistently when comparing platforms.`
- `get_game_rank_markets`: `List the countries, app-store categories, stores, and ranking types where a game appeared on a chart during a date range. Returns each obse…`
- `get_game_summary`: `Summarize creatives, ad plans, lifetime exposure references and Google Play net download increments within a date range. download_increment…`
- `get_game_trend`: `Get daily game delivery trends for the requested date range. Creative and ad counts represent delivery activity; exposure is a lifetime ref…`
- `get_material_detail_v2`: `Get creative summary, media and owning-game information using a complete material_reference returned by this service. Resolve the exact mat…`
- `get_material_rank`: `Get rising or evergreen creative rankings by period and optional primary/secondary category. Return rank, material_reference, video media,…`
- `get_material_reuse_clues`: `Find directly recorded reuse relationships for a creative material_reference. Return related games, developers, first/last appearances, rel…`
- `get_reference_image_search_results`: `Get completed reference-image search results. If the job is still running, returns polling guidance. Example: 'Show the matches from my ref…`
- `get_reference_image_search_status`: `Get the processing status of a reference-image search job. Example: 'Is my reference-image search finished yet?'`
- `get_similar_materials_v2`: `Find visually similar creatives from a complete material_reference using stored video-content vectors. Return games, developers, delivery d…`
- `get_store_first_seen_games`: `Find games first observed in official daily app-store charts, defined per package, platform, country, category and rank type. This is not a…`
- `get_store_game_rank`: `Get official Google Play or iPhone App Store free, paid or grossing charts by day, week or month and official category. country_code must b…`
- `get_store_game_rank_filter`: `Get valid platforms, rank types, periods, countries, official categories and dates for official app-store rankings, including the latest Go…`
- `get_store_game_rank_trend`: `Get game-level official daily chart trends using a game token or an app identifier resolved through the official package mapping. Best mode…`
- `report_capability_gap`: `Record an unmet analysis need for future product improvements when existing tools cannot satisfy the request. Include the missing capabilit…`
- `resolve_game_by_identifier`: `Resolve an Android package name or numeric iOS app ID to game tokens and identity. Return all matching regional editions, ordered by lifeti…`
- `search_games`: `Search mobile games by name or category across global markets. Return identity, active ads and creatives in the last 30 days, and their lif…`
- `search_materials_by_filter`: `Search creatives by game category, creative labels, country, platform and format. Each label dimension accepts one standard value; differen…`
- `search_materials_by_keyword`: `Search creative copy and labels by keyword, optionally within a game and date range. Return opaque material references and direct video add…`
- `search_materials_distribution`: `Aggregate ad-plan and creative counts/shares by delivery platform and country using discovery filters. Return aggregates only. Each creativ…`
- `search_materials_v2`: `Discover creatives by games, countries, platforms, formats, languages, aspect ratio, duration, device, quality and discovery dates. Each re…`
- `submit_reference_image_search`: `Submit a reference-image similarity search as an asynchronous job. Use this when the user provides a directly downloadable public HTTPS ima…`

## Changes

- 2026-09-10: [count changed, description changed, schema changed, tool added, tool removed](../../deltas/2026-09-10/611783010d7bc9a98efa.json): `30 tool(s) added; 8 tool(s) removed; 13 field(s) changed`
- 2026-09-08: [count changed, description changed, tool added](../../deltas/2026-09-08/611783010d7bc9a98efa.json): `1 tool(s) added; 2 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.creativescope.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
