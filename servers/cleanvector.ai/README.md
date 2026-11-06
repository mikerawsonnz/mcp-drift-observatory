# cleanvector.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/cleanvector.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://cleanvector.ai/api/mcp` | 11 | [`c208fb14df92`](41a01cdfc8691335024d.json) | 2026-09-22 |

## Tools at `https://cleanvector.ai/api/mcp`

- `download_logo_kit`: `Return a completed logo kit as an embedded ZIP resource. Includes three SVGs, three PNGs and palette.json. MCP output is capped at 2048px;…`
- `download_png`: `Return the finished artwork as a PNG image (free on all plans). Use after a task succeeded. For larger exports up to 8192px, use the png_ur…`
- `download_svg`: `Return the finished artwork as SVG markup. Use after a task succeeded.`
- `generate_illustration`: `Generate professional, editable SVG artwork from a text prompt: illustrations, icons, stickers and mascot scenes. The result is real vector…`
- `generate_logo`: `Generate a professional vector logo as editable SVG, delivered as a brand kit: the original mark, black and white variants, transparent PNG…`
- `get_account`: `Current plan and credit balance. Costs: vectorize 1, generate/enhance 4, logo 8 credits. PNG and SVG downloads are free on every plan.`
- `get_task`: `Fetch the current status of a task. Status is one of queued, processing, succeeded, failed. A succeeded task includes the result with downl…`
- `list_mascots`: `List the user's ready-to-use mascots (consistent characters). Pass a mascot id to generate_illustration to place that character in a new sc…`
- `list_tasks`: `List the user's most recent tasks, newest first.`
- `vectorize_image`: `Convert a raster image (PNG/JPG/WebP, max 5 MB) into a clean, editable SVG. Provide image_url or image_base64. no_background defaults to tr…`
- `wait_for_task`: `Block until a task settles (succeeded/failed) or the timeout passes. Preferred over polling get_task in a loop. Generation typically takes…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://cleanvector.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
