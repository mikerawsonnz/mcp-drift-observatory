# registry.run.mcp.com.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/registry.run.mcp.com.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://registry.run.mcp.com.ai/mcp` | 3 | [`063f85af5293`](4dc30d6123c983482fa2.json) | 2026-08-20 |

## Tools at `https://registry.run.mcp.com.ai/mcp`

- `getV01Servers`: `List MCP servers - Returns a list of all registered MCP servers`
- `getV01ServersServerNameVersions`: `List all versions of an MCP server - Returns all available versions for a specific MCP server, ordered by publication date (newest first)`
- `getV01ServersServerNameVersionsVersion`: `Get specific MCP server version - Returns detailed information about a specific version of an MCP server. Use the special version 'latest'…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://registry.run.mcp.com.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
