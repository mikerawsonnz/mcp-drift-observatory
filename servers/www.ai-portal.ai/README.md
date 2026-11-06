# www.ai-portal.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.ai-portal.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.ai-portal.ai/mcp` | 4 | [`27404b0ef26c`](255166daf0e577d5062e.json) | 2026-08-20 |

## Tools at `https://www.ai-portal.ai/mcp`

- `get_latest_news`: `Latest curated GenAI news items from AI-Portal, refreshed every weekday morning.`
- `list_regulations`: `List AI regulations and their compliance status (EU AI Act, ISO 42001, and more), including jurisdiction, effective dates, key requirements…`
- `list_releases`: `List AI model and product releases tracked by AI-Portal, newest first. Filter by category, provider, year, or landmark releases only.`
- `search_glossary`: `Search AI-Portal's glossary of AI/GenAI terms. Returns term, definition, category, and a usage example.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.ai-portal.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
