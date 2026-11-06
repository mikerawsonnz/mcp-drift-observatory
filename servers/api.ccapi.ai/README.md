# api.ccapi.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.ccapi.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.ccapi.ai/mcp/music` | 6 | [`ae1d9b21817b`](5f66abe7b09e06a00165.json) | 2026-08-20 |
| `https://api.ccapi.ai/mcp/image` | 6 | [`98b1a889f9fc`](69c267bf0c781574cb5f.json) | 2026-08-20 |
| `https://api.ccapi.ai/mcp/video` | 4 | [`bf78ea8ef5ed`](723f6b66686ad4401de9.json) | 2026-08-26 |
| `https://api.ccapi.ai/mcp/text` | 4 | [`c20e8b920d96`](bb7b2286ad7980dbb095.json) | 2026-08-20 |
| `https://api.ccapi.ai/mcp` | 11 | [`c871faee99ad`](e54b696689b950e4d564.json) | 2026-08-26 |

## Tools at `https://api.ccapi.ai/mcp/music`

- `extend_music`: `Continue an existing song from a given timestamp, producing a longer version. Requires the clip_id of a previously generated song, which ap…`
- `generate_lyrics`: `Write song lyrics from a description, without generating audio. Useful as a first step before generate_music with custom=true, so the user…`
- `generate_music`: `Generate a song with vocals or instrumental. Two modes: simple (custom=false) where you describe the song and the model writes the lyrics,…`
- `get_balance`: `Report the remaining and used balance for this CCAPI key. Useful before starting an expensive batch of generations, or to explain a quota f…`
- `get_task`: `Check the status of an asynchronous generation task submitted by generate_video, generate_music, generate_lyrics, extend_music, or generate…`
- `list_models`: `List the AI models this CCAPI key can actually call, with their capability category and the MCP tool that drives them. Call this before gen…`

## Tools at `https://api.ccapi.ai/mcp/image`

- `edit_image`: `Edit existing images according to an instruction, using the dedicated image edit endpoint. Provide at least one source image. For pure text…`
- `generate_image`: `Generate an image from a text prompt, optionally guided by reference images (image-to-image). Returns image URLs directly. Most models fini…`
- `get_balance`: `Report the remaining and used balance for this CCAPI key. Useful before starting an expensive batch of generations, or to explain a quota f…`
- `get_task`: `Check the status of an asynchronous generation task submitted by generate_video, generate_music, generate_lyrics, extend_music, or generate…`
- `list_models`: `List the AI models this CCAPI key can actually call, with their capability category and the MCP tool that drives them. Call this before gen…`
- `upscale_image`: `Increase the resolution of an existing image 2x with ccapi-upscale-v1. Input must be between 256x256 and 1024x1024 and under 5 MB; for larg…`

## Tools at `https://api.ccapi.ai/mcp/video`

- `generate_video`: `Generate a video from a text prompt, optionally driven by reference images (image-to-video, first/last frame). This is asynchronous: it ret…`
- `get_balance`: `Report the remaining and used balance for this CCAPI key. Useful before starting an expensive batch of generations, or to explain a quota f…`
- `get_task`: `Check the status of an asynchronous generation task submitted by generate_video, generate_music, generate_lyrics, extend_music, or generate…`
- `list_models`: `List the AI models this CCAPI key can actually call, with their capability category and the MCP tool that drives them. Call this before gen…`

## Tools at `https://api.ccapi.ai/mcp/text`

- `chat_completion`: `Send a conversation to any text model available through CCAPI (Claude, GPT, Gemini, DeepSeek, GLM, MiniMax, Kimi, Qwen…) and get the reply.…`
- `get_balance`: `Report the remaining and used balance for this CCAPI key. Useful before starting an expensive batch of generations, or to explain a quota f…`
- `get_task`: `Check the status of an asynchronous generation task submitted by generate_video, generate_music, generate_lyrics, extend_music, or generate…`
- `list_models`: `List the AI models this CCAPI key can actually call, with their capability category and the MCP tool that drives them. Call this before gen…`

## Tools at `https://api.ccapi.ai/mcp`

- `chat_completion`: `Send a conversation to any text model available through CCAPI (Claude, GPT, Gemini, DeepSeek, GLM, MiniMax, Kimi, Qwen…) and get the reply.…`
- `edit_image`: `Edit existing images according to an instruction, using the dedicated image edit endpoint. Provide at least one source image. For pure text…`
- `extend_music`: `Continue an existing song from a given timestamp, producing a longer version. Requires the clip_id of a previously generated song, which ap…`
- `generate_image`: `Generate an image from a text prompt, optionally guided by reference images (image-to-image). Returns image URLs directly. Most models fini…`
- `generate_lyrics`: `Write song lyrics from a description, without generating audio. Useful as a first step before generate_music with custom=true, so the user…`
- `generate_music`: `Generate a song with vocals or instrumental. Two modes: simple (custom=false) where you describe the song and the model writes the lyrics,…`
- `generate_video`: `Generate a video from a text prompt, optionally driven by reference images (image-to-video, first/last frame). This is asynchronous: it ret…`
- `get_balance`: `Report the remaining and used balance for this CCAPI key. Useful before starting an expensive batch of generations, or to explain a quota f…`
- `get_task`: `Check the status of an asynchronous generation task submitted by generate_video, generate_music, generate_lyrics, extend_music, or generate…`
- `list_models`: `List the AI models this CCAPI key can actually call, with their capability category and the MCP tool that drives them. Call this before gen…`
- `upscale_image`: `Increase the resolution of an existing image 2x with ccapi-upscale-v1. Input must be between 256x256 and 1024x1024 and under 5 MB; for larg…`

## Changes

- 2026-08-26: [schema changed](../../deltas/2026-08-26/723f6b66686ad4401de9.json): `8 field(s) changed`
- 2026-08-26: [schema changed](../../deltas/2026-08-26/e54b696689b950e4d564.json): `8 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.ccapi.ai/mcp/music"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
