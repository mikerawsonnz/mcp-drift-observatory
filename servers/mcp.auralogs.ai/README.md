# mcp.auralogs.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.auralogs.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.auralogs.ai/mcp` | 7 | [`be54a73d5521`](f8f5ec9ee8248bd49fa1.json) | 2026-08-20 |

## Tools at `https://mcp.auralogs.ai/mcp`

- `get_analysis`: `Get a single analysis by id (diagnosis, suggested fix, PR link if any).`
- `get_log`: `Get a single log row by id, with full context (stack, metadata).`
- `get_project`: `Get a project by id. Must match the read key's scoped project.`
- `list_analyses`: `List active analyses for the scoped project. Archived analyses (triaged from the dashboard) are excluded by default; pass include_archived=…`
- `list_logs`: `List logs for the scoped project, optionally filtered by level/since/until.`
- `list_projects`: `List projects accessible to the current read key (one project for v1).`
- `search_logs`: `Full-text search log messages for the scoped project.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.auralogs.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
