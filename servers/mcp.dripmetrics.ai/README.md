# mcp.dripmetrics.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.dripmetrics.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.dripmetrics.ai/mcp` | 6 | [`3b9bd7490d68`](d9e26b1beb3a76601f01.json) | 2026-09-16 |

## Tools at `https://mcp.dripmetrics.ai/mcp`

- `compute_portfolio_var`: `Paid via x402 ($0.05 per request). Computes empirical and/or normal parametric VaR for a crypto portfolio. Provide either weights + portfol…`
- `compute_spread_greeks`: `Paid via x402 ($0.05 per request). Nets Black-76 greeks across up to 6 Deribit BTC option legs and returns a spot×vol scenario P&L grid. In…`
- `describe_metric`: `Free. Returns full details for one metric id from list_metrics: parameters, request/response schemas, price, and how to fetch it.`
- `get_metric`: `Paid via x402 (up to $0.25 per request; exact price per metric in list_metrics). Fetches any GET metric by id with query parameters. Withou…`
- `get_payment_requirements`: `Free. Dry-runs a metric request without payment and returns the exact x402 challenge the API issues (accepted networks, asset, amount, payT…`
- `list_metrics`: `Free. Lists every DripMetrics metric endpoint with its id, family, HTTP method, USD price, and summary. Use describe_metric for parameter d…`

## Changes

- 2026-09-16: [schema changed](../../deltas/2026-09-16/d9e26b1beb3a76601f01.json): `10 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.dripmetrics.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
