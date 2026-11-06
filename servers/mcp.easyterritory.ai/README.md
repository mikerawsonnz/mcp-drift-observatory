# mcp.easyterritory.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.easyterritory.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.easyterritory.ai` | 47 | [`fcb8fdef040b`](8d279300fedac539bc59.json) | 2026-10-11 |

## Tools at `https://mcp.easyterritory.ai`

- `account_build`: `Builds territories that follow an account column, such as rep name or territory code from CRM: each part goes to the group holding most of…`
- `analyze`: `Computes territory statistics for one or more alignments, i.e. how balanced the territories are and how alignments compare: account counts,…`
- `analyze_routes`: `Returns the total hours for each of the routes calculate_route has drawn: drive hours, dwell hours, route_workload_hours (provider drive ti…`
- `auto_build`: `Partitions ingested account points into balanced sales territories with equal workload, metric, or count over a part layer (e.g. ZIPs) and…`
- `calculate_route`: `Sequences and drives a set of stops, e.g. a technician from home to the depot, then the day's calls, and back home: returns the order, road…`
- `cluster_points`: `Groups the points of one ingested layer into balanced clusters directly, with no ZIP or part layer and no territory alignment. Writes group…`
- `configure_map`: `Updates durable map settings on the Territory Solution and refreshes the live map: project_name (map heading), loaded_part_layers ([] hides…`
- `create_territory_from_parts`: `Creates one leaf territory from a list of part_ids (e.g. a committed map selection), in a new alignment or an existing one (tal_id). With m…`
- `delete_route`: `Route delete: removes one whole route from the Territory Solution and the open map, in one synchronous call. Needs route_id or the route's…`
- `delete_tal`: `Deletes one whole territory alignment (TAL: 'the territory layer', 'all territories') from the Territory Solution and the open map, in one…`
- `delete_territory`: `Deletes one leaf territory from an alignment; its parts become unassigned. Needs tal_id, territory_id (the leaf id or its exact unique disp…`
- `direct_build`: `Builds territories from known part-to-territory assignments (a ZIP-to-territory sheet or file, including a three-level region/district/terr…`
- `discover_intent`: `Maps a free-text territory request to a workflow. Read-only keyword routing; no compute. Returns intent_category, the recommended tool orde…`
- `ensure_map_viewer`: `Reports whether the person has the map open (viewer_status.connected) for a map_session_id from get_map_visualization, waiting up to wait_s…`
- `ep_graph_traverse`: `Traverses the EMEP knowledge graph from a topic file (e.g. 'workflows/realign-by-selection.md') to related guidance, up to 'depth' hops. Re…`
- `ep_list_topics`: `Lists EMEP topics grouped by type (concept, workflow, interface, troubleshooting, decision). Optional 'type' filter.`
- `ep_search`: `Semantic search over the EZT MCP Expert Pack (EMEP): workflow guidance, concepts, interfaces, and common mistakes. Returns ranked markdown…`
- `export_geojson`: `Exports the territory solution as one GeoJSON file to share, archive, or open in EasyTerritory Designer: territory polygons with part_ids,…`
- `extract_tal_branch`: `Extracts one regional branch of a hierarchical alignment (by branch_rollup_territory_id or branch_territory_path) into its own Territory So…`
- `ezt`: `Plain-language orchestrator: takes request (the goal) and runs the matching workflow in one call, optionally with csv_file (a host file par…`
- `geocode_address`: `Geocodes a list of customer addresses to coordinates with match confidence, without loading them as a point layer. Accepts address/address_…`
- `get_guidance`: `Returns the EZT MCP operating guide: the cross-tool workflow order and shared rules (result.text, same text as the server instructions), re…`
- `get_map_selection`: `Returns the most recent committed selection on an open map session (map_session_id): part_layer, part_ids, and selection_task_id when the s…`
- `get_map_visualization`: `Opens the interactive territory map (Map Component) and returns map_url and map_session_id. Opens a blank map, or shows the latest state of…`
- `get_part_selection`: `Returns the state of a map selection task (selection_task_id from request_part_selection, or active_selection_task_id in ezt://map-sessions…`
- `import_geojson`: `Opens a GeoJSON FeatureCollection (plain points, or a territory file this server produced, plain or gzip/zip) as a Territory Solution and r…`
- `ingest_accounts`: `Account ingest: loads account or location rows (CRM records, a CSV, a spreadsheet) as point data on a named point layer of the Territory So…`
- `isochrone_build`: `Draws the area reachable by driving from one or more origins within a time or distance budget (drive-time area, service area, catchment) an…`
- `load_analysis_panel`: `Shows a completed analyze result in the open map's analysis dock (single or compare). Needs map_session_id and the analyze task_id/job_id o…`
- `query_parts`: `Returns attributes (no geometry) for parts of a part layer listed at ezt://part-layers. Takes exactly one of filter (e.g. {state_abbr: TX})…`
- `realign`: `Moves ZIPs or other parts (typed ids or ones selected on the map) from one territory into another within one alignment (tal_id): a ZIP move…`
- `reintegrate_branch`: `Merges an edited branch (proposal Territory Solution from extract_tal_branch) back into the master. Needs branch_metadata and expected_mast…`
- `request_account_upload`: `Stages account rows for ingest_accounts and returns upload_handle, csv_headers, and suggested_ingest args with a geocode_plan. Four ways in…`
- `request_assignment_upload`: `Stages part-to-territory assignment rows (e.g. a ZIP-to-territory spreadsheet with Postal Code plus Territory/Region/Division) for direct_b…`
- `request_part_selection`: `Lets the person adjust boundaries by picking parts (e.g. ZIPs) on the map: puts the open map into select mode on a part_layer, for purpose…`
- `schedule_visits`: `Schedules recurring visits: expands each account's cadence (e.g. every 7 days, twice a month) across a horizon and packs the visits into da…`
- `seed_build`: `Grows one territory outward from a seed {longitude, latitude} over a part layer until it holds a target: {type: location_count, value: N} o…`
- `set_map_state`: `Changes the open map's session state: mode, active alignment (active_tal_id), pending job reference, or camera (center [longitude, latitude…`
- `show_map_overlay`: `Shows or hides something on the open map from a plain request ('add US zip codes', 'hide the zips', 'show my accounts') or overlay_kind (pa…`
- `submit_feedback`: `Sends product feedback to EasyTerritory: a blocked or partial workflow, a workaround, a confusing response, or a missing capability. Return…`
- `tasks_cancel`: `Tool equivalent of the native MCP tasks/cancel, listed for clients without the Tasks capability. Requests cooperative cancellation of a tas…`
- `tasks_get`: `Tool equivalent of the native MCP tasks/get, listed for clients without the Tasks capability. Returns the Task status document for a task_i…`
- `tasks_result`: `Tool equivalent of the native MCP tasks/result, listed for clients without the Tasks capability. Returns the originating tool's terminal re…`
- `territory_merge`: `Merges a pair of adjacent territories and rebalances the rest of the alignment with minimal disruption (N to N-1 territories), e.g. when a…`
- `territory_rebalance`: `Rebalances an existing alignment after the account data changed, keeping it as close to the current alignment as possible. Needs source_tal…`
- `territory_split`: `Territory split: divides one territory (e.g. an oversized one) into two while changing the rest of the alignment as little as possible (N t…`
- `workflow_advisor`: `Returns the next tool call for a multi-step workflow, given where the workflow stands. Read-only state machine; executes nothing. intent_ca…`

## Changes

- 2026-10-11: [schema changed](../../deltas/2026-10-11/8d279300fedac539bc59.json): `1 field(s) changed`
- 2026-10-10: [description changed, schema changed](../../deltas/2026-10-10/8d279300fedac539bc59.json): `159 field(s) changed`
- 2026-10-09: [annotation changed, description changed, field changed](../../deltas/2026-10-09/8d279300fedac539bc59.json): `283 field(s) changed`
- 2026-10-07: [description changed](../../deltas/2026-10-07/8d279300fedac539bc59.json): `6 field(s) changed`
- 2026-10-06: [description changed, schema changed](../../deltas/2026-10-06/8d279300fedac539bc59.json): `57 field(s) changed; signals: imperative_language_introduced` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.easyterritory.ai"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
