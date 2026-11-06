# mcp.arvx.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.arvx.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.arvx.ai/mcp` | 3 | [`19039080d174`](83ef4f6317f7a5f8175c.json) | 2026-10-31 |

## Tools at `https://mcp.arvx.ai/mcp`

- `arvx_get_access`: `How to get access to ARVX: the signup link to give the person, what they must do themselves, the price, and how to add their key to this co…`
- `arvx_record_summary`: `When someone asks what is held about them: returns every item in a saved record in plain words. Needs the record and both people's emails.…`
- `arvx_run_reading`: `Run a Reading on two people from the emails between them. Send at least 3 emails written by the user and 3 by the other person, oldest firs…`

## Changes

- 2026-10-31: [schema changed](../../deltas/2026-10-31/83ef4f6317f7a5f8175c.json): `79 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.arvx.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
