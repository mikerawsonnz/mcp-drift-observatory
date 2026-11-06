# api.chinaapi.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.chinaapi.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.chinaapi.ai/mcp` | 4 | [`bdecb9ac3727`](657f296b5d7089cccb6a.json) | 2026-10-06 |

## Tools at `https://api.chinaapi.ai/mcp`

- `chinaapi_estimate_cost`: `Estimate the USD cost of a workload on one model from its published per-meter prices: Standard, and Paid where it is lower. Pass quantities…`
- `chinaapi_get_model`: `Get one model by its exact ID: base URL and endpoints, the Standard and Paid price snapshot per meter with the time it was read and the pri…`
- `chinaapi_get_recipe`: `Get a runnable request for one model — endpoint, headers, JSON body or multipart form, a curl command, and for video the polling step — exa…`
- `chinaapi_list_models`: `List the models ChinaAPI serves, optionally filtered by capability, task, maker or a model-ID substring. Each entry has the exact model ID,…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.chinaapi.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
