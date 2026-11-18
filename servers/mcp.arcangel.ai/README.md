# mcp.arcangel.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.arcangel.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.arcangel.ai/trademark` | 9 | [`f256832a9aad`](51dbd3b220397cebf7d7.json) | 2026-11-18 |

## Tools at `https://mcp.arcangel.ai/trademark`

- `check_trademark`: `Check whether a brand, product or company name is available as a trademark. Searches the USPTO register and scores similar marks by conflic…`
- `create_company`: `Save a company profile in the signed-in Arcangel account, as on the Companies page, so it can own trademark applications. Every field excep…`
- `get_trademark_application`: `Show what a trademark application draft still needs before it can be signed and paid for: missing fields, files to upload (logo, specimens)…`
- `get_trademark_check`: `Get the result of a trademark check that was still running, or the next part of a long full report. Pass the search_id that check_trademark…`
- `list_companies`: `List the companies saved in the signed-in Arcangel account, with their ids. Call this before asking for company details on a trademark appl…`
- `start_trademark_application`: `Start a US trademark application on Arcangel AI as a draft in the signed-in user's account. Pass what is known (the mark, goods or services…`
- `suggest_nice_classes`: `Suggest trademark (Nice) classes for a description of goods or services, e.g. "mobile app for booking yoga classes".`
- `update_company`: `Change fields on a saved company (id from list_companies). Only the fields passed change. A draft already linked to the company picks up th…`
- `update_trademark_application`: `Fill in or change fields on a trademark application draft (owner, address, mark details, classes, use dates, statements). Only fields passe…`

## Changes

- 2026-11-18: [count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-18/51dbd3b220397cebf7d7.json): `3 tool(s) added; 20 field(s) changed`
- 2026-11-17: [count changed, field changed, tool added](../../deltas/2026-11-17/51dbd3b220397cebf7d7.json): `3 tool(s) added; 6 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.arcangel.ai/trademark"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
