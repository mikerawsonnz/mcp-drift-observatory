# mcp.arcangel.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.arcangel.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.arcangel.ai/trademark` | 3 | [`276c5a2b363e`](51dbd3b220397cebf7d7.json) | 2026-11-15 |

## Tools at `https://mcp.arcangel.ai/trademark`

- `check_trademark`: `Check whether a brand, product or company name is available as a trademark. Searches the USPTO register and scores similar marks by conflic…`
- `get_trademark_check`: `Get the result of a trademark check that was still running, or the next part of a long full report. Pass the search_id that check_trademark…`
- `suggest_nice_classes`: `Suggest trademark (Nice) classes for a description of goods or services, e.g. "mobile app for booking yoga classes".`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.arcangel.ai/trademark"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
