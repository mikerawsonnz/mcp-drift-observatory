# license-changes-mcp.ottobot2025.workers.dev: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/license-changes-mcp.ottobot2025.workers.dev.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://license-changes-mcp.ottobot2025.workers.dev/mcp` | 2 | [`57ab361ec946`](1d92d2001f9c8f6fab69.json) | 2026-09-08 |

## Tools at `https://license-changes-mcp.ottobot2025.workers.dev/mcp`

- `check_license_history`: `Has this contractor's licence changed? Returns every status transition observed in the state board's own published file since 2026-07-17 --…`
- `recent_license_changes`: `What changed lately across a state: licences that lapsed, were reinstated, or appeared for the first time, newest first, optionally narrowe…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://license-changes-mcp.ottobot2025.workers.dev/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
