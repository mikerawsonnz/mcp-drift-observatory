# lenny-rachitsky.run.mcp.com.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/lenny-rachitsky.run.mcp.com.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://lenny-rachitsky.run.mcp.com.ai/mcp` | 8 | [`1d976a05cd8f`](7977c4621303270751f4.json) | 2026-08-20 |

## Tools at `https://lenny-rachitsky.run.mcp.com.ai/mcp`

- `getEpisodes`: `List episodes - Lists episodes with parsed frontmatter (guest, title, duration, youtube_url, etc.) and their canonical resource URIs.`
- `getEpisodesGuest`: `Get an episode card (metadata + key URIs)`
- `getEpisodesGuestChunks`: `List chunk descriptors for an episode - Returns chunk boundaries and URIs for chunk retrieval. Chunks may be computed on-demand using size/…`
- `getEpisodesGuestChunksChunkIdtxt`: `Get a specific transcript chunk as plain text`
- `getEpisodesGuestMetadatajson`: `Get episode metadata as JSON (frontmatter)`
- `getEpisodesGuestTranscriptformat`: `Get transcript in a specific format - Returns the transcript in the requested format: - md: markdown (may include or exclude frontmatter ba…`
- `getSearch`: `Search episodes and transcripts - Searches across metadata (D1) and transcript text (Vectorize). Returns matches as resources, including pe…`
- `postSearch`: `Search episodes and transcripts (POST body) - Same search as GET /search, but parameters are provided in the request body. This is useful f…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://lenny-rachitsky.run.mcp.com.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
