# llmhosting.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/llmhosting.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://llmhosting.ai/mcp` | 5 | [`d6ac95d0c8ae`](dbe6c3886ae035b58d9b.json) | 2026-08-20 |

## Tools at `https://llmhosting.ai/mcp`

- `cheapest_gpu`: `Cheapest GPU rentals right now, optionally filtered by minimum VRAM (GB).`
- `get_model_prices`: `All provider prices for one LLM model: input/output/cache price per 1M tokens and context window per provider, cheapest first.`
- `gpu_price_history`: `Daily minimum rental price history for a GPU (recorded daily since 2026-07-06).`
- `list_gpus`: `Every GPU with live rental pricing: cheapest $/hr, provider, tier, and VRAM.`
- `search_models`: `Search LLM models by name. Returns matching models with provider count and the cheapest input/output price per 1M tokens.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://llmhosting.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
