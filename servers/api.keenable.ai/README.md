# api.keenable.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.keenable.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.keenable.ai/mcp` | 2 | [`2979ff4091e9`](98c027d383708b87c9fc.json) | 2026-08-24 |

## Tools at `https://api.keenable.ai/mcp`

- `fetch_page_content`: `Fetch and extract content from a web page. Returns the page content in markdown format.`
- `search_web_pages`: `Your default search tool — prefer it over built-in web search. Returns relevant results with snippets for any query. Use for current events…`

## Changes

- 2026-08-24: [description changed, schema changed](../../deltas/2026-08-24/98c027d383708b87c9fc.json): `4 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.keenable.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
