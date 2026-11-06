# cerebrium.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/cerebrium.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://cerebrium.ai/docs/mcp` | 3 | [`40abd384d6a5`](4f7d9ea5115fd6450d8e.json) | 2026-10-24 |

## Tools at `https://cerebrium.ai/docs/mcp`

- `query_docs_filesystem_cerebrium`: `Run a read-only shell-like query against a virtualized, in-memory filesystem rooted at '/' that contains ONLY the Cerebrium documentation p…`
- `search_cerebrium`: `Search across the Cerebrium knowledge base to find relevant information, code examples, API references, and guides. Use this tool when you…`
- `submit_feedback`: `Report a problem with this documentation site so the docs team can fix it. Use when a documentation page is incorrect, outdated, confusing,…`

## Changes

- 2026-10-24: [annotation changed, field changed](../../deltas/2026-10-24/4f7d9ea5115fd6450d8e.json): `4 field(s) changed`
- 2026-09-16: [description changed, schema changed](../../deltas/2026-09-16/4f7d9ea5115fd6450d8e.json): `3 field(s) changed; signals: url_introduced`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://cerebrium.ai/docs/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
