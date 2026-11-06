# synap-mcp.maximem.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/synap-mcp.maximem.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://synap-mcp.maximem.ai/mcp` | 4 | [`94d0f9fb1e14`](371c947d14316af7bb11.json) | 2026-08-27 |

## Tools at `https://synap-mcp.maximem.ai/mcp`

- `check_memory_status`: `Check whether a logged exchange has finished processing. Pass the ingestion_id returned by log_exchange. Returns the processing status and…`
- `list_recent_memories`: `List recent things remembered about this user. Useful for debugging or to confirm that memory is working. Pass user_id to scope to one pers…`
- `log_exchange`: `After each user message, send the exchange here so it can be remembered. You do not need to decide what is important, just forward the user…`
- `recall_context`: `Before replying, call this to recall anything already known about this user from past conversations. Use the user's latest message as the q…`

## Changes

- 2026-08-27: [description changed, schema changed](../../deltas/2026-08-27/371c947d14316af7bb11.json): `10 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://synap-mcp.maximem.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
