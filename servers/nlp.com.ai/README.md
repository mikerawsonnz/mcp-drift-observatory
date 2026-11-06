# nlp.com.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/nlp.com.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://nlp.com.ai/mcp` | 3 | [`91320e4bfaa7`](fd1e4eca243388f9429c.json) | 2026-10-20 |

## Tools at `https://nlp.com.ai/mcp`

- `get_model`: `Return the complete curated record for one model or model-family release, addressed by the slug returned from search_models or recent_model…`
- `recent_models`: `Return the newest curated open-weight model release records, optionally limited to releases on or after an ISO 8601 date.`
- `search_models`: `Search curated open-weight model release records by model name, developer, license, parameter or context description, and technical feature…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://nlp.com.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
