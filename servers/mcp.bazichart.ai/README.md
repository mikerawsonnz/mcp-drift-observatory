# mcp.bazichart.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.bazichart.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.bazichart.ai/mcp` | 2 | [`17a41c0ea07c`](8c0310faf30ab6446407.json) | 2026-11-18 |

## Tools at `https://mcp.bazichart.ai/mcp`

- `cast_bazi`: `Calculate BaZi from a known local Gregorian birth time and birthplace. Returns four pillars, luck cycles, ten gods, hidden stems and time c…`
- `cast_ziwei`: `Calculate a Ziwei natal chart. Overseas birthplaces (including HK/Macao/Taiwan) use local true solar time; longitude required. Returns pala…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.bazichart.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
