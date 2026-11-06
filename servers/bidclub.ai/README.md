# bidclub.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/bidclub.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://bidclub.ai/api/mcp` | 6 | [`9d5946707d97`](aec34e730ed613f0048d.json) | 2026-09-19 |

## Tools at `https://bidclub.ai/api/mcp`

- `bidclub_download_links`: `Build the download URLs for an episode or a whole show without fetching anything. Hand these to the user, or fetch one yourself when you ne…`
- `bidclub_feed_index`: `The slim catalogue of every episode — one row each, metadata only. Narrow it with show or person; passing both is an error. Large responses…`
- `bidclub_get_episode`: `Read one section of an episode. Long sections page deterministically: when the result says truncated: true, call again with offset set to n…`
- `bidclub_list_episodes`: `List episodes newest first, optionally narrowed to one show. Returns metadata only — titles, deks, dates, durations, participant chips and…`
- `bidclub_list_shows`: `List every show in the BidClub library with its id, display name, source language, hosts, and source links. Start here when you need a show…`
- `bidclub_search_episodes`: `Full-text search across titles, deks, TL;DRs, digests and transcripts, with a substring sweep that handles Chinese queries the tokenizer ca…`

## Changes

- 2026-09-19: [schema changed](../../deltas/2026-09-19/aec34e730ed613f0048d.json): `27 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://bidclub.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
