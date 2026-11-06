# mcp.deployit.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.deployit.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.deployit.ai/demo` | 3 | [`3b0099276670`](9e88b811adac08e1dd47.json) | 2026-09-01 |

## Tools at `https://mcp.deployit.ai/demo`

- `ask_product_expert`: `Ask a question about "deployit" and get an answer verified against its live source code and git history. Use it for anything about product…`
- `get_recent_changes`: `Instant list of recent changes to "deployit" — the semantic changelog derived from its commits. No AI processing: responds in under a secon…`
- `server_info`: `Describe this MCP server: which product it answers for, which repositories back it, and how fresh the underlying code index is. Instant (no…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.deployit.ai/demo"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
