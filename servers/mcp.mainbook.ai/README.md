# mcp.mainbook.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.mainbook.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.mainbook.ai/mcp` | 4 | [`ec80c927ed4b`](ad68c3ad3a12e6b5a954.json) | 2026-08-22 |

## Tools at `https://mcp.mainbook.ai/mcp`

- `convert_bank_statement`: `Convert one PDF bank statement through the complete MainBook workflow: create a job, upload, start, poll, and return structured data. This…`
- `get_balance`: `Return total, reserved, and available MainBook credits. Every value is measured in PDF pages.`
- `get_conversion`: `Get the current state of one MainBook conversion. When successful, return JSON inline or save XLSX/CSV locally over stdio. HTTP mode return…`
- `list_conversions`: `List one cursor page of conversion jobs visible to the MainBook account. Pass the returned next_cursor to continue.`

## Changes

- 2026-08-22: [schema changed](../../deltas/2026-08-22/ad68c3ad3a12e6b5a954.json): `22 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.mainbook.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
