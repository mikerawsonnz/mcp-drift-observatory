# docs.bondren.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/docs.bondren.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://docs.bondren.ai/mcp` | 2 | [`a599132ed519`](12e31449e4419f5ba847.json) | 2026-11-25 |

## Tools at `https://docs.bondren.ai/mcp`

- `get_doc`: `Read the canonical Markdown of one docs page by id, or a single section when an anchor is supplied. Returns the page/section URL, content h…`
- `search_docs`: `Search the Bondren public docs corpus for ranked sections matching a query. Limit defaults to 5, and the ranked result set is the top 10 ma…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://docs.bondren.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
