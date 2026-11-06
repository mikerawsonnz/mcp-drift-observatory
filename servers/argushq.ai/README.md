# argushq.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/argushq.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://argushq.ai/api/mcp` | 5 | [`b55effdbc5a0`](5df8f88bf142530fb9ab.json) | 2026-08-20 |

## Tools at `https://argushq.ai/api/mcp`

- `get_company_history`: `Every FDA warning letter, recall, approval, and 483 citation Argus HQ has recorded for a given company, by its Argus HQ company slug (e.g.…`
- `get_recall_by_lot`: `Finds every FDA recall record that references a specific product lot number.`
- `get_warning_letter`: `Direct lookup of an FDA warning letter. Accepts either the FDA reference number printed in the letter itself (e.g. "320-26-65") or the fda.…`
- `list_recent_actions`: `The most recent published FDA warning letters, recalls, approvals, and 483 citations across all streams.`
- `search_enforcement`: `Full-text search across all 1,000+ Argus HQ FDA enforcement pages (warning letters, recalls, approvals, 483 inspections) by keyword, produc…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://argushq.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
