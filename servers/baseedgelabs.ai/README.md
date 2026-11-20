# baseedgelabs.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/baseedgelabs.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://baseedgelabs.ai/mcp` | 4 | [`febf07b1242f`](8130ce63d6f7c63f14b8.json) | 2026-11-20 |

## Tools at `https://baseedgelabs.ai/mcp`

- `export_preset`: `Returns download links to one preset's two files, each with import steps. "tradingview": a flat settings file keyed by input label, for Tra…`
- `get_preset`: `Returns one preset in full: its summary and Strategy Tester results, the Strategy Tester properties to set (initial capital, commission, sl…`
- `list_presets`: `Finds presets: saved settings of a strategy for one instrument and chart timeframe. Each result has its preset_id, strategy, instrument, ti…`
- `list_strategies`: `Lists every BaseEdge Labs trading strategy for TradingView: its strategy_id, name, page on baseedgelabs.ai, whether it is free or paid, how…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://baseedgelabs.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
