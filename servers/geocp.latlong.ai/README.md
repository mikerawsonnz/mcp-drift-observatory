# geocp.latlong.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/geocp.latlong.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://geocp.latlong.ai/mcp` | 6 | [`bbcfb577600b`](dc0acd210c0fe6a3d649.json) | 2026-09-03 |

## Tools at `https://geocp.latlong.ai/mcp`

- `get_capabilities`: `Return the server's capability matrix (supported map types, geo types, output formats, and classification methods).`
- `get_index`: `Get computed index scores for regions. Returns rankings + render_map_input payload. MODES: - mode="rank" (default): Top N regions ranked by…`
- `list_geographies`: `List supported India geographic region types (state, district, city, AC, PC, SCR, PINCODE) with coverage notes.`
- `list_indices`: `List all available computed indices with descriptions and supported geographic levels.`
- `render_map`: `Render a map from structured JSON data. Returns SVG markup by default with metadata (render_id, join_summary, unmatched_geos, warnings). Se…`
- `validate_map`: `Validate whether a dataset can be rendered as a map. Runs geo matching and config resolution without generating an image. Returns valid/war…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://geocp.latlong.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
