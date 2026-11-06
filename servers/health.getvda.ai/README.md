# health.getvda.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/health.getvda.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://health.getvda.ai/mcp` | 5 | [`ce7d160e265b`](b14a3b8c52338fed49cb.json) | 2026-08-20 |

## Tools at `https://health.getvda.ai/mcp`

- `health_check`: `Full monitoring cycle: re-discover from the seed, merge with the saved map, check HTTP/TCP/SSL/DNS, detect latency anomalies, roll dependen…`
- `health_discover`: `FREE dry run: discover everything a seed would monitor — subdomains, compose services, ports, dependency chains — without monitoring or sto…`
- `health_exclude`: `FREE: add .healthignore patterns for a seed. Applies next cycle.`
- `health_history`: `Timeline of status changes for a seed over the last N hours.`
- `selftest`: `FREE, no payment required. Runs this agent's real capability on a fixed canned input and returns the genuine result, an honest assertion gr…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://health.getvda.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
