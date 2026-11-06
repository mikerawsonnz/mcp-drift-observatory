# aiphotoanimator.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/aiphotoanimator.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://aiphotoanimator.ai/api/mcp` | 10 | [`33b0ff4a6695`](3a58aab8be84c56ca46b.json) | 2026-10-30 |

## Tools at `https://aiphotoanimator.ai/api/mcp`

- `animate_photo`: `Turn photo(s) into a short video. With 'effect' (from list_effects) the effect decides the motion; without it the photo is animated followi…`
- `create_image`: `Generate a new image from text, or edit photo(s) following instructions (change background, outfit, style, lighting, combine several photos…`
- `create_video`: `Generate a short video (5 seconds, 720p, with sound) from a text description only, no photo needed. Costs credits. Returns a task_id; poll…`
- `edit_video`: `Edit an existing video clip (MP4, up to 15 seconds, 50 MB) following instructions: put the person from a photo into the clip, change outfit…`
- `get_credits`: `Remaining credits and plan of the connected account.`
- `get_image`: `Check an image task from create_image or restore_photo. status is pending, success (image_url ready) or failed (credits refunded).`
- `get_video`: `Check a generation task. status is pending, success (video_url ready) or failed (credits refunded).`
- `list_effects`: `List video effect templates (dance, sports, meme scenes, etc.). Use the returned 'effect' id with animate_photo. 'photos' is how many photo…`
- `list_my_videos`: `The user's most recent video generations, newest first.`
- `restore_photo`: `Repair an old or damaged photo: remove scratches, dust, creases and fading, recover sharp faces, keep everyone exactly as they are. Optiona…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://aiphotoanimator.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
