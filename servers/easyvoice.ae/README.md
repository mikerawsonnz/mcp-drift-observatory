# easyvoice.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/easyvoice.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://easyvoice.ae/api/mcp` | 7 | [`2aeacd40cba6`](193ec671f4b3c2ec3e1e.json) | 2026-10-27 |

## Tools at `https://easyvoice.ae/api/mcp`

- `clone_voice`: `Enroll a custom cloned voice from an audio sample (async). Requires a Pro or active 7-day pass key. Provide exactly one of audio_base64 or…`
- `create_podcast`: `Create a two-host (A/B) podcast episode as an async job. Requires a Pro subscription key. Up to 60 segments; combined text up to 30,000 cha…`
- `generate_long_form`: `Generate long-form narration (up to 500,000 characters ≈ 9 hours of audio) as an async job. Requires a Pro subscription key. Kokoro narrati…`
- `get_job_status`: `Check the status of a long-form, podcast or tts job owned by this key. Returns status plus audio URL(s) when completed. Audio links are not…`
- `get_usage`: `Check this API key's plan and usage. Free keys see today's used/remaining characters (shared 5,000/day pool, resets at midnight UTC), the 2…`
- `list_voices`: `List all 66 EasyVoice catalog voices (id, name, language, accent, gender, free/pro tier) plus this key's cloned voices. Call this before te…`
- `text_to_speech`: `Convert text to a downloadable MP3 or WAV audio file with one of EasyVoice's 66 neural voices or your ready cloned voice_* ids (Pro or acti…`

## Changes

- 2026-10-27: [description changed, schema changed](../../deltas/2026-10-27/193ec671f4b3c2ec3e1e.json): `3 field(s) changed`
- 2026-10-14: [description changed](../../deltas/2026-10-14/193ec671f4b3c2ec3e1e.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://easyvoice.ae/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
