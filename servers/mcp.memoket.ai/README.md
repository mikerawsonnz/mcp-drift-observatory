# mcp.memoket.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.memoket.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.memoket.ai/mcp` | 7 | [`bf131223154f`](c3736a8a43cc205a9f06.json) | 2026-08-20 |

## Tools at `https://mcp.memoket.ai/mcp`

- `get_brief`: `[content_fetch] Per-conversation compact report body for the given conversation_ids using Brief -> Summary -> Standard, where Standard is t…`
- `get_conversations`: `[metadata_query] Conversation-level metadata for the given conversation_ids: id, title, started_at, ended_at, duration_seconds, participant…`
- `get_summaries`: `[content_fetch] Per-conversation summary body. With summary_ids, fetch exact summary reports from search_recordings. With conversation_ids…`
- `get_transcripts`: `[content_fetch] Verbatim transcript of ONE recording by conversation_id. Paginated (offset / next_offset) — page through for more.`
- `get_transcripts_by_participant`: `[content_fetch] Transcript lines associated with participant_ids in conversation_ids. Turns participant metadata into transcript evidence f…`
- `list_conversations`: `[metadata_query] List recordings by time window / participants. Returns id, title, started_at, ended_at, duration_seconds, participants, la…`
- `search_recordings`: `[search] Unified recording search. Runs bounded searches over transcript lines, topic segments, memory atoms, participant metadata, titles,…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.memoket.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
