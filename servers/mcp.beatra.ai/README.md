# mcp.beatra.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.beatra.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.beatra.ai/mcp` | 36 | [`fd2a0989a42a`](4f93d616eb97e76f800a.json) | 2026-11-12 |

## Tools at `https://mcp.beatra.ai/mcp`

- `beatra.assets.upload`: `Create a short-lived upload grant for an image, audio, or video file. Follow the returned HTTP PUT instructions; its response returns the a…`
- `beatra.audio.process`: `Process one audio file: trim, loop to a length, fade, normalize loudness, convert format, split into stems (vocals and accompaniment, or si…`
- `beatra.avatars.list`: `List the portraits this account saved as avatars for talking-presenter videos, the default first, each with its image artifact and paired v…`
- `beatra.avatars.save`: `Save one image already in this account as a named avatar the user can reuse in later sessions. Call only after the user agreed to save it a…`
- `beatra.images.edit`: `Edit images[0] as the base image; later images are ordered references and optional regions use normalized coordinates. Omit model unless th…`
- `beatra.images.generate`: `Generate one to four images from text without source images. Omit model unless the user explicitly requests one; call beatra.models.list be…`
- `beatra.images.transform`: `Transform one to four ordered reference images with a prompt; when canvas aspect is source, the last reference anchors the ratio. Omit mode…`
- `beatra.images.understand`: `Answer questions about one to eight ordered images, each limited to 10 MiB. Upload a local image with beatra.assets.upload first and pass i…`
- `beatra.installations.register`: `Idempotently register the current Skill package for this authenticated installation, with optional channel, install source, network route a…`
- `beatra.models.list`: `List models currently selectable for one Beatra generation capability, including live supported controls, constraints, customer credit pric…`
- `beatra.music.edit`: `Revise a music track made by beatra.music.generate or an uploaded song: extend it, replace a time range, add vocals to an instrumental, or…`
- `beatra.music.generate`: `Generate songs or instrumentals from a prompt, lyrics, or reference audio; optionally set a target length in seconds, reuse a saved persona…`
- `beatra.social.execute`: `Look up public social data and create a task. This billable call consumes Beatra credits and creates an asynchronous task. Submit exactly o…`
- `beatra.social.tools.get`: `Read one public social data tool, including its arguments, schema_hash, and credit price. This call is not billable.`
- `beatra.social.tools.search`: `Search public social data tools by platform, keyword, or capability_family. This call is not billable.`
- `beatra.speech.prepare_script`: `Use before beatra.speech.synthesize to make speech sound natural and human. Beatra's Smart Voice Director reads the text and the user's opt…`
- `beatra.speech.synthesize`: `Synthesize speech using a Beatra voice ID. This billable call consumes Beatra credits and creates an asynchronous task. Submit exactly once…`
- `beatra.speech.validate`: `Check a speech request before paying for it: parse the markup, list warnings, count weighted characters, and return the credit price. This…`
- `beatra.tasks.cancel`: `Cancel a task created by this MCP connection. In-flight work is canceled only when the remote stop is confirmed; a 409 means continue polli…`
- `beatra.tasks.get`: `Read a Beatra task created by this MCP connection.`
- `beatra.tasks.list`: `List recent Beatra tasks created by this MCP connection.`
- `beatra.videos.animate`: `Animate a first-frame image, optionally with driving audio; use interpolate instead when both first and last frames are supplied. Call beat…`
- `beatra.videos.compose`: `Join your own video clips into one MP4 with optional narration, ducked music, and burned-in subtitles. Set keep_audio on a clip to keep tha…`
- `beatra.videos.edit`: `Edit one source video by instruction, with optional multimodal references; do not use this to extend a clip. Input plus output duration may…`
- `beatra.videos.enhance_prompt`: `Enhance a creative video prompt from optional image, video, or audio context. This creates an asynchronous text-only task and does not gene…`
- `beatra.videos.extend`: `Generate footage immediately before or after one source clip. Use edit to alter existing frames. Duration is a required integer final retur…`
- `beatra.videos.generate`: `Generate from text when there is no source image or video. Supports optional driving audio on compatible models. Omit model unless the user…`
- `beatra.videos.generate_from_references`: `Generate from ordered image, video, and audio references. Use animate for one strict opening image and interpolate for strict first and las…`
- `beatra.videos.interpolate`: `Generate toward a required last frame, optionally constrained by a first frame and driving audio. Use animate when only a first frame exist…`
- `beatra.videos.understand`: `Answer questions about one video limited to 50 MiB and 360 seconds. Upload a local video with beatra.assets.upload first and pass it as an…`
- `beatra.voices.activate`: `Activate a cloned voice whose clone result says activation is required (status pending_activation). Voices that are already ready, includin…`
- `beatra.voices.clone`: `Clone a voice from a clean single-speaker sample. With the default engine (omit model or use 'auto') the cloned voice is ready for speech a…`
- `beatra.voices.list`: `List preset and tenant-owned voices available for speech synthesis. By default only voices ready for speech are listed; pass status to incl…`
- `beatra.voices.update`: `Rename one of this account's cloned voices, or make a voice (cloned or preset) the account's default. Call only when the user asked for tha…`
- `beatra.wallet.get`: `Read the current Beatra credit balance for this account, including the next expiring batch. Also returns how many unfinished creations this…`
- `beatra.wallet.ledger`: `List this account's credit ledger newest first: charges, refunds, top-ups, and expiry. This call is read-only and does not charge. Page wit…`

## Changes

- 2026-11-12: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-12/4f93d616eb97e76f800a.json): `2 tool(s) added; 107 field(s) changed`
- 2026-11-09: [count changed, schema changed, tool added](../../deltas/2026-11-09/4f93d616eb97e76f800a.json): `1 tool(s) added; 3 field(s) changed`
- 2026-11-07: [description changed, schema changed](../../deltas/2026-11-07/4f93d616eb97e76f800a.json): `72 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-11-04: [schema changed](../../deltas/2026-11-04/4f93d616eb97e76f800a.json): `7 field(s) changed`
- 2026-10-31: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-31/4f93d616eb97e76f800a.json): `1 tool(s) added; 163 field(s) changed; signals: length_more_than_doubled`
- 2026-10-29: [description changed, schema changed](../../deltas/2026-10-29/4f93d616eb97e76f800a.json): `49 field(s) changed; signals: length_more_than_doubled`
- 2026-10-28: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-28/4f93d616eb97e76f800a.json): `1 tool(s) added; 100 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.beatra.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
