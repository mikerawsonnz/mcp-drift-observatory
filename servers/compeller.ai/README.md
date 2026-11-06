# compeller.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/compeller.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://compeller.ai/api/mcp` | 30 | [`3693804a4f2a`](df883af943a7d995a879.json) | 2026-08-20 |

## Tools at `https://compeller.ai/api/mcp`

- `ack_lighting_cue`: `REACT/BAE acknowledgement for a launch_id. Idempotently records whether the executor accepted or rejected the cue and which executor observ…`
- `cancel_compel`: `Cancel an in-progress compel. Dequeues it if still queued, otherwise cancels any active external (AI provider) tasks and transitions it to…`
- `create_compel`: `Create a Compeller generation job from primary audio media and optional reference media. Returns compel id, status, and links to track prog…`
- `create_compel_from_music`: `Create a compel from a selected Deezer preview track. If the user provides an audio file instead, upload that file and use create_compel.`
- `delete_webhook`: `Delete a webhook endpoint by id. Removes the registration and stops future deliveries.`
- `get_account_credits`: `Get the authenticated account's render-minute balance and plan: minutes remaining (free + paid), monthly allowance, plan code, and whether…`
- `get_capabilities`: `Get Compeller platform capabilities, supported features, and API version.`
- `get_compel`: `Get the current status, progress, and details of a Compeller generation job.`
- `get_lighting_cue`: `Fetch a single live lighting cue by its launch_id, including resolved variables, launch_contract, and REACT feedback.`
- `get_pricing`: `Get current Compeller subscription plans and pricing.`
- `get_rendering`: `Get details of a specific video rendering.`
- `launch_lighting_cue`: `Launch a starter lighting effect onto a stage as a live cue (e.g. "gobo-cycle on the stage's 7R beams at speed 0.5"). Pass effect_id (from…`
- `list_compels`: `List all Compeller generation jobs for the authenticated account, newest first.`
- `list_lighting_cues`: `List the live (non-stopped) lighting cues REACT is executing, including each cue's launch_id, resolved variables, launch_contract, and feed…`
- `list_lighting_effects`: `List the COM-497 starter lighting effects available to launch as cues (e.g. "gobo-cycle", "x-move", "dimmer-pulse"). Each effect carries an…`
- `list_renderings`: `List all video renderings for a specific compel.`
- `list_styles`: `List available visual styles for Compeller video generation.`
- `list_webhooks`: `List all webhook endpoints registered for the authenticated account. Secrets are never returned by this tool.`
- `register_webhook`: `Register an HTTPS endpoint to receive signed push notifications for compel lifecycle events (compel.ready when renderable, compel.completed…`
- `report_lighting_cue`: `REACT/BAE report-back for cue status, active variables, skipped bindings, capability misses, last_frame_at, and errors.`
- `rotate_webhook_secret`: `Mint a new HMAC-SHA256 signing secret for a registered webhook endpoint. The previous secret is invalidated immediately - integrators must…`
- `search_compels`: `Search Compeller generation jobs by title for the authenticated account.`
- `search_media`: `Search and list uploaded media files for the authenticated account.`
- `search_music`: `Search Deezer preview tracks by song, artist, or album. Use this when the user provides a song string but no MP3/WAV/FLAC file.`
- `set_lighting_cue_variables`: `Update variables on a live cue (e.g. change cycle speed or intensity mid-show). Only the variables you pass change; the rest keep their cur…`
- `start_render`: `Start rendering a READY compel with default configuration so an agent can continue to final MP4 without opening the browser UI.`
- `stop_lighting_cue`: `Stop a live cue by its launch_id. Idempotent - the cue is marked stop-requested so REACT drops it on its next refresh.`
- `test_webhook_delivery`: `Synchronously POST a synthetic webhook.test event to a registered endpoint. Uses the same HMAC-SHA256 signature as real deliveries, runs th…`
- `update_webhook`: `Update one or more mutable fields on a registered webhook endpoint: url, events, active. At least one of these must be provided. Validation…`
- `upload_media`: `Get upload instructions for media files (audio, images, video). Returns the upload URL and required headers. Requires API token authenticat…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://compeller.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
