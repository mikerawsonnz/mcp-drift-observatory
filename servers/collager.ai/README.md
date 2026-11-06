# collager.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/collager.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://collager.ai/mcp` | 5 | [`02633d1cc1ae`](4292e5f20a018863d4db.json) | 2026-10-18 |

## Tools at `https://collager.ai/mcp`

- `get_shape_collage`: `Returns the status and the watermarked preview of a collage made with make_shape_collage, by its id (clg_...). Use when make_shape_collage…`
- `list_collage_shapes`: `Lists the shapes make_shape_collage can draw (hearts of 27-164 photos, numbers, words, I love you, circle, star, flower, grid, your own mas…`
- `list_mosaic_styles`: `Shows the looks of a Collager.ai photo mosaic (one large picture made of hundreds or thousands of small photos) with example images: soft c…`
- `make_shape_collage`: `Builds a photo collage in the shape of a heart, a number (age, anniversary, year), a word, a star, a flower and more from the user's photos…`
- `start_photo_mosaic`: `Gives the link where the user builds a photo mosaic: one main photo recreated from many small photos (best with 100-2000 photos - family ar…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://collager.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
