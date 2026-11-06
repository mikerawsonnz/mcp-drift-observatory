# arclan.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/arclan.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://arclan.ai/mcp` | 4 | [`60d213d22489`](0b01ebd7cd8a49a80df5.json) | 2026-08-20 |

## Tools at `https://arclan.ai/mcp`

- `get_server`: `Get full details for a specific MCP server. Pass the server name (e.g. "GitHub", "Brave Search"), registry ID slug, or endpoint URL. Return…`
- `query_registry`: `Search the Arclan registry for MCP servers. By default returns only connectable servers (active, mcp_partial, auth_gated). Use status=stdio…`
- `recommend_server`: `Get ranked MCP server recommendations for a task. Returns servers scored by production safety, keyword relevance, registry score, latency,…`
- `report_server`: `Submit an agent usage report for an MCP server. Reports are aggregated and influence registry trust scores. Call this after using an MCP se…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://arclan.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
