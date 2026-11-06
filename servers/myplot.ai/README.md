# myplot.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/myplot.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://myplot.ai/mcp` | 2 | [`b63732a8818e`](ccf15d4de703af8bde2d.json) | 2026-08-20 |

## Tools at `https://myplot.ai/mcp`

- `get_property_report`: `Get comprehensive property risk data plus an AI-written narrative analysis for any US address. Includes all 22 data sources from get_proper…`
- `get_property_risk_data`: `Get comprehensive property risk data for any US address from 22 federal data sources. Returns flood zone (FEMA), earthquake risk (USGS), ai…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://myplot.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
