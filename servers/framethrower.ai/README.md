# framethrower.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/framethrower.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://framethrower.ai/api/mcp` | 4 | [`37870fb08691`](407f92f6717749fc8a66.json) | 2026-09-01 |

## Tools at `https://framethrower.ai/api/mcp`

- `find_by_craft`: `Find frames by specific cinematography craft attributes — lens character, shot size, visual style, setting, time of day, director, or year…`
- `find_similar`: `Find frames visually/semantically similar to a given frame id (from a prior result). Use this to pull more references like one the user sho…`
- `get_frame_details`: `Get the full metadata + preview thumbnail + full-resolution image URL + depth map URL + link for a single frame id. The depth map is precom…`
- `search_frames`: `Search the FrameThrower cinematography reference library by concept, mood, color, composition, or scene. Returns reference frames with film…`

## Changes

- 2026-09-01: [description changed](../../deltas/2026-09-01/407f92f6717749fc8a66.json): `2 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://framethrower.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
