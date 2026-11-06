# mcp.bithuman.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.bithuman.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.bithuman.ai/mcp` | 3 | [`e7f6572a526d`](9188611bf3bbaff0377b.json) | 2026-10-30 |

## Tools at `https://mcp.bithuman.ai/mcp`

- `list_characters`: `List the bitHuman house characters that can speak. Each has an id (pass it as 'character' to make_character_video or talk_to_character), a…`
- `make_character_video`: `Make a short video of one bitHuman house character saying 'text' word for word, in its own voice. Returns video_url (an MP4 that plays inli…`
- `talk_to_character`: `Open a live voice conversation with one bitHuman house character in a player in the chat. The user presses Start and speaks through the mic…`

## Changes

- 2026-10-30: [description changed](../../deltas/2026-10-30/9188611bf3bbaff0377b.json): `1 field(s) changed`
- 2026-10-17: [schema changed](../../deltas/2026-10-17/9188611bf3bbaff0377b.json): `2 field(s) changed`
- 2026-10-14: [description changed, field changed, schema changed](../../deltas/2026-10-14/9188611bf3bbaff0377b.json): `9 field(s) changed; signals: length_more_than_doubled`
- 2026-10-10: [annotation changed, count changed, schema changed, tool removed](../../deltas/2026-10-10/9188611bf3bbaff0377b.json): `1 tool(s) removed; 2 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.bithuman.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
