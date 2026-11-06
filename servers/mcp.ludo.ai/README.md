# mcp.ludo.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.ludo.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.ludo.ai/mcp` | 31 | [`0b225098bfa9`](2c068d79c8f49a1d9416.json) | 2026-09-03 |

## Tools at `https://mcp.ludo.ai/mcp`

- `animate3DModel`: `Generate text-driven skeletal animations for an already-rigged 3D model. Pass the rigged GLB in 'model' (URL or base64) and a motion 'promp…`
- `animate3DModelPreset`: `Apply a curated animation preset to an already-rigged 3D model (retargeting). Pass the rigged GLB in 'model' (URL or base64) and a 'preset_…`
- `animateSprite`: `Animate a static sprite into a spritesheet driven by a motion text prompt (image-to-spritesheet): supply an initial_image (URL or base64) p…`
- `animateSpriteKeyframes`: `Animate a sprite through up to three fixed keyframes - initial_image, middle_image and final_image (each a URL or base64) - producing a spr…`
- `cancelApiJob`: `Cancel a queued job you started through the API or MCP and refund its credits. Jobs that are already running cannot be canceled (409). Retu…`
- `create3DModel`: `Convert a single source image into a textured 3D model (image-to-3D). The job result is a downloadable GLB model_url plus an array of snaps…`
- `createAmbiance`: `Produce a looping background ambiance soundscape from a text description, such as "windy forest at dusk" or "busy tavern interior". The job…`
- `createAudioTransform`: `Remix an existing audio sample (a sound effect, ambiance, or music clip) into a variation guided by a text prompt, for example turning a tr…`
- `createImage`: `Generate game-art images from a text prompt alone, selecting an image_type (e.g. sprite) and optionally art_style, perspective, and aspect_…`
- `createMusic`: `Produce a piece of music from a text description, such as "epic orchestral battle theme" or "calm piano melody", with optional lyrics. The…`
- `createSoundEffect`: `Produce a short sound effect (SFX) from a text description, such as "laser gun firing" or "footsteps on gravel". The job result is a single…`
- `createSpeech`: `Convert text to speech by cloning the voice from an audio sample you provide (voice-cloning text-to-speech). Both text and sample are requi…`
- `createSpeechPreset`: `Convert text to speech using a named built-in preset voice, with optional emotion and language settings. Both text and voice_preset_id are…`
- `createVideo`: `Generate a short video clip from a source image and a motion text prompt (image-to-video). The job result is the video URL and its actual d…`
- `createVideoFromReferences`: `Generate a video from 1-5 reference images and a text prompt (references-to-video). Unlike createVideo, which animates a single source imag…`
- `createVoice`: `Design a new voice from a character description (such as "deep-voiced warrior" or "cheerful young girl") and have it speak a short line of…`
- `editImage`: `Modify an existing image according to text instructions: supply a source image (URL or base64) and a prompt describing the changes (e.g. "a…`
- `editSpritesheet`: `Edit a previously generated spritesheet: re-prompt its underlying animation (edit_mode "prompt"), extend the frame beyond its borders ("out…`
- `editVideo`: `Edit a previously generated video with a text prompt and optional reference images (video-to-video). Pass the video 'url' you received from…`
- `generatePose`: `Re-pose an existing sprite into a new target pose while preserving the character, taking a source image (URL or base64), a pose name (or "O…`
- `generateWithStyle`: `Generate new images that match the visual style of a reference image: supply a style_image (URL or base64) plus a text prompt describing wh…`
- `getApiJob`: `Poll the status of a generation job started by any tool. Every tool returns '{id, status}'; call getApiJob with that id until status is 'su…`
- `listAnimationPresets`: `List the available animation presets along with their perspectives and the eight supported compass directions (N, NE, E, SE, S, SW, W, NW).…`
- `listApiJobs`: `List the generation jobs you started through the API or MCP, most recent first. Web-app jobs are not included. This is a free read-only loo…`
- `listGenerations`: `List your generation history across the API and the web app - filter by type, source (api/web/all), text search, and date range. Returns {i…`
- `removeBackground`: `Remove the background from a single image, returning the subject isolated on a transparent background. Supply the source image (URL or base…`
- `rigModel`: `Rig a 3D model: generate a skeleton and skin weights for an existing GLB so it can be animated. Accepts a URL or base64-encoded GLB in 'mod…`
- `rotateSprite`: `Re-render an existing sprite from a different camera viewpoint while keeping the same character and pose, taking a source image (URL or bas…`
- `transferMotion`: `Transfer motion from a reference video or a named animation preset onto a static sprite image, producing an animated spritesheet that mimic…`
- `upscaleVideo`: `Upscale a previously generated video to twice its resolution (2x). Pass the video 'url' you received from 'createVideo', 'createVideoFromRe…`
- `validateApiKeyEndpoint`: `Validates an API key. Returns 200 if valid, 403 if invalid.`

## Changes

- 2026-09-03: [schema changed](../../deltas/2026-09-03/2c068d79c8f49a1d9416.json): `24 field(s) changed`
- 2026-09-01: [description changed, schema changed](../../deltas/2026-09-01/2c068d79c8f49a1d9416.json): `35 field(s) changed`
- 2026-08-31: [count changed, description changed, schema changed, tool added, tool removed](../../deltas/2026-08-31/2c068d79c8f49a1d9416.json): `4 tool(s) added; 5 tool(s) removed; 50 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-08-28: [schema changed](../../deltas/2026-08-28/2c068d79c8f49a1d9416.json): `30 field(s) changed`
- 2026-08-26: [description changed, schema changed](../../deltas/2026-08-26/2c068d79c8f49a1d9416.json): `72 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.ludo.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
