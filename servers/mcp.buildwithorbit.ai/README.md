# mcp.buildwithorbit.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.buildwithorbit.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.buildwithorbit.ai/mcp` | 2 | [`e7d0f9578101`](bdeac8e6c93a6d8f06d6.json) | 2026-09-10 |

## Tools at `https://mcp.buildwithorbit.ai/mcp`

- `integrate`: `Get integration details for public endpoints and MCPs from 'search' results. Provide a 'task' describing what you want to accomplish and up…`
- `search`: `Find and evaluate public API endpoints and MCPs that match your query. Set 'q' to a natural language query, keywords, an API name, or a que…`

## Changes

- 2026-09-10: [description changed, schema changed](../../deltas/2026-09-10/bdeac8e6c93a6d8f06d6.json): `6 field(s) changed`
- 2026-09-03: [description changed, schema changed](../../deltas/2026-09-03/bdeac8e6c93a6d8f06d6.json): `11 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.buildwithorbit.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
