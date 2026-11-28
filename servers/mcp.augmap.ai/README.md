# mcp.augmap.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.augmap.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.augmap.ai/mcp` | 11 | [`49eb81f68546`](84a4400d881dca99e201.json) | 2026-11-28 |

## Tools at `https://mcp.augmap.ai/mcp`

- `map_create`: `Create a map of places in the continental US. Returns map_id and map_url.`
- `map_edit_lists`: `Create, update (rename, change kind, pin a saved list to a plan list) or delete lists. A plan list's date goes in its name ("Sat, Oct 3 · A…`
- `map_edit_places`: `Add, update, move, remove (park in rejected) or restore places. Each op result has the list_id and kind of the list it used.`
- `map_favorites`: `Read the traveler's favorite places: the lists they keep in their Augmap account, and their organizations' lists, each place with place_id,…`
- `map_get_state`: `Read a map: lists, places, save_state, version, pending_changes.`
- `map_list`: `List the traveler's saved maps, and maps shared with them, with their map_id and map_url.`
- `map_save`: `Save a map to the traveler's account.`
- `map_search_places`: `Find places and street addresses in the continental US for an existing map_id. Returns places and fields_granted per query.`
- `map_set_view`: `Pan/zoom the live map.`
- `map_share`: `Publish or unpublish a saved map's public view link, create, list or revoke links that let other people view it or join it as editors, chan…`
- `map_update`: `Change a map's title, context, travel mode, interests, day noun or whether it routes between stops.`

## Changes

- 2026-11-28: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-28/84a4400d881dca99e201.json): `1 tool(s) added; 17 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.augmap.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
