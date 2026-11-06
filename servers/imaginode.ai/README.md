# imaginode.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/imaginode.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://imaginode.ai/api/mcp` | 4 | [`0edfab38f459`](774474760a0ac274791e.json) | 2026-08-26 |

## Tools at `https://imaginode.ai/api/mcp`

- `generate_image`: `Generate an image from a text prompt (optionally with input images for editing or reference). Waits for the result and returns the image UR…`
- `generate_video`: `Start a video generation from a text prompt (optionally with a start image). Returns immediately with a request_id and the cost in credits:…`
- `get_generation_status`: `Check a generation started with generate_video (or a generate_image that timed out). Returns running, completed (with output URLs) or faile…`
- `list_models`: `List the available AI models with their kind (image, video), default cost in credits (1 credit = $0.012, or €0.01 when billed in euros) and…`

## Changes

- 2026-08-26: [description changed](../../deltas/2026-08-26/774474760a0ac274791e.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://imaginode.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
