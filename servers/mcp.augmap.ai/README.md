# mcp.augmap.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.augmap.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.augmap.ai/mcp` | 10 | [`c16f1879d1b4`](84a4400d881dca99e201.json) | 2026-11-06 |

## Tools at `https://mcp.augmap.ai/mcp`

- `map_create`: `Create a map of places in the continental US. Returns map_id and map_url.`
- `map_edit_lists`: `Create, update (rename, change kind, pin a saved list to a plan list) or delete lists. A plan list's date goes in its name ("Sat, Oct 3 · A…`
- `map_edit_places`: `Add, update, move, remove (park in rejected) or restore places. Each op result has the list_id and kind of the list it used.`
- `map_get_state`: `Read a map: lists, places, save_state, version, pending_changes.`
- `map_list`: `List the traveler's saved maps, and maps shared with them, with their map_id and map_url.`
- `map_save`: `Save a map to the traveler's account.`
- `map_search_places`: `Find places and street addresses in the continental US for an existing map_id. Returns places and fields_granted per query.`
- `map_set_view`: `Pan/zoom the live map.`
- `map_share`: `Create, list or revoke links that let other people view a saved map or join it as editors, change a link's role, or list and manage the peo…`
- `map_update`: `Change a map's title, context, travel mode, interests, day noun or whether it routes between stops.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.augmap.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
