# meetlark.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/meetlark.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://meetlark.ai/mcp` | 6 | [`306dc4cf05ce`](b0383e0953495657267f.json) | 2026-08-20 |

## Tools at `https://meetlark.ai/mcp`

- `meetlark_close_poll`: `Close a poll to stop accepting new votes. Use the admin token from poll creation.`
- `meetlark_create_poll`: `Create a scheduling poll to find a time that works for a group. Returns an admin URL (keep private) and a participation URL (share with par…`
- `meetlark_get_admin_view`: `Get full poll details including all votes and participants. This is the only way to see who voted and how they voted. Returns poll info, ti…`
- `meetlark_get_results`: `Get poll details and available time slots using a participation token. Returns the poll title, description, status, and time slots -- but N…`
- `meetlark_reopen_poll`: `Reopen a previously closed poll to accept votes again. Use the admin token from poll creation.`
- `meetlark_vote`: `Cast a vote on a scheduling poll. Each time slot can be voted yes, maybe, or no. Requires participant name and email. Use the participation…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://meetlark.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
