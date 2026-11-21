# mcp.agentapigate.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.agentapigate.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.agentapigate.ai/mcp` | 4 | [`ab1054ed853c`](db2d4296f359addb82c6.json) | 2026-11-21 |

## Tools at `https://mcp.agentapigate.ai/mcp`

- `call_endpoint`: `Execute an endpoint and return compact LLM-ready output (-80% context tokens).`
- `get_account_status`: `Inspect paid_usd, bonus_usd, rate limit, and active sub-key caps.`
- `get_endpoint_schema`: `Get JSON input schema, price, and sample params for an endpoint_id.`
- `search_endpoints`: `Search 136 real-time APIs across x, search, social, commerce, b2b, finance, local, intel. Returns id, price_usd, p50_ms, summary.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.agentapigate.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
