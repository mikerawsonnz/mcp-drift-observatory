# mcp.agentapigate.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.agentapigate.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.agentapigate.ai/mcp` | 4 | [`8ca3d569f400`](db2d4296f359addb82c6.json) | 2026-11-27 |

## Tools at `https://mcp.agentapigate.ai/mcp`

- `call_endpoint`: `Execute any endpoint (e.g. search.google.web, search.google.news, web.extract.markdown, youtube.video.transcript) and return compact LLM-re…`
- `get_account_status`: `Inspect paid_usd, bonus_usd, rate limit, and active sub-key caps.`
- `get_endpoint_schema`: `Get JSON input schema, price, and sample params for an endpoint_id.`
- `search_endpoints`: `Search 145 real-time APIs across x, search, social, commerce, b2b, finance, local, intel. Returns id, price_usd, p50_ms, summary.`

## Changes

- 2026-11-27: [annotation changed, description changed, schema changed](../../deltas/2026-11-27/db2d4296f359addb82c6.json): `75 field(s) changed; signals: length_more_than_doubled`
- 2026-11-26: [description changed](../../deltas/2026-11-26/db2d4296f359addb82c6.json): `1 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.agentapigate.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
