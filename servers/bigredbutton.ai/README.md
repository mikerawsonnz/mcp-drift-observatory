# bigredbutton.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/bigredbutton.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://bigredbutton.ai/api/mcp` | 3 | [`b235aab62389`](2bd0b518c9a318a73c48.json) | 2026-11-26 |

## Tools at `https://bigredbutton.ai/api/mcp`

- `discover_supply`: `Find existing supply by service and area. Ask only for missing details returned as needs_input. Explicit browse=countries lists A–Z countri…`
- `list_providers`: `Read current providers and profiles from a discovered service page. No phone numbers.`
- `prepare_message`: `Only when the user explicitly asks to message a chosen provider, prepare a Big Red profile link carrying their draft; its Message button us…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://bigredbutton.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
