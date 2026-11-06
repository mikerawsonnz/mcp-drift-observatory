# everymcp.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/everymcp.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://everymcp.ai/mcp` | 3 | [`827dabcc5917`](596527375e2a6753d159.json) | 2026-10-06 |

## Tools at `https://everymcp.ai/mcp`

- `get_install_config`: `Return a ready-to-run install command, or the exact configuration fragment, for one MCP server and one client. This data comes from the Off…`
- `get_server`: `Return the full registry record for one MCP server, its verification facts, and which clients it can be installed into. This data comes fro…`
- `search_tools`: `Search the public MCP server universe by what you want a server to do. Returns compact summaries; call get_server for a full record. This d…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://everymcp.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
