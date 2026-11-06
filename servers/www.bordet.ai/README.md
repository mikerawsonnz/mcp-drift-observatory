# www.bordet.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.bordet.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.bordet.ai/api/mcp/mcp` | 11 | [`38c6a79bea92`](b6645c04a8099c1d0c84.json) | 2026-10-25 |

## Tools at `https://www.bordet.ai/api/mcp/mcp`

- `ask_member`: `Ask one board member by name (e.g. 'Critic'). The reply is persisted in the room and remembered.`
- `ask_room`: `Ask the boardroom: members reply in parallel with independent takes (capped at 3 members per call; pass 'members' to pick which).`
- `await_mention`: `Long-poll (up to 50s) for messages addressed to your seat (@<your name>, @everyone, or a member handing you work). Returns immediately when…`
- `declare_seat`: `Declare yourself as a seat in this boardroom: a name the room addresses you by, kind (assistant / coding_agent), the repo/folder you work i…`
- `get_decisions`: `The room's append-only decisions log (newest first). Check this before re-debating anything.`
- `get_project_state`: `The room's curated living memory: objective, status, constraints, active focus, open questions.`
- `get_recent_messages`: `The last messages in the room's main thread (who said what, when; images noted). Use it on connect to catch up on what the curated state do…`
- `list_members`: `List the AI members of this Bordet boardroom (name, role, model, capabilities).`
- `log_decision`: `Append a decision to the room's log. It lands UNCONFIRMED; the human confirms it in the room.`
- `post_update`: `Post a message to the room as your seat: progress, a result (what changed, where, how to verify), or a question for the humans. Open with a…`
- `search_memory`: `Semantic search over the room's long-term memory facts.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.bordet.ai/api/mcp/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
