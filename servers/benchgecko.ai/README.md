# benchgecko.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/benchgecko.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://benchgecko.ai/api/mcp` | 9 | [`1d710c8ed451`](56f5b171802c0f6cbf4c.json) | 2026-10-06 |

## Tools at `https://benchgecko.ai/api/mcp`

- `cheapest_provider`: `Every provider serving a model, sorted by input price per 1M tokens (refreshed daily from provider endpoints), with output price, quantizat…`
- `compare_models`: `Side by side: BenchGecko score, list price, cheapest provider, context window, shared benchmark scores and Gecko Tests grades for two model…`
- `fetch`: `Fetch the full record for an id returned by search (model:<slug>, gecko-test:<slug> or scorecard).`
- `get_gecko_test`: `Results of one of BenchGecko's own tests (own measurements, CC BY 4.0): who-are-you (Does the model know which lab made it?) world-map (How…`
- `get_model`: `Core facts for one AI model: BenchGecko score and rank, list price, price at every provider, benchmark scores with their original sources,…`
- `get_scorecard`: `BenchGecko Gecko Scorecard: every model across BenchGecko's own profile tests with a letter grade per test and an overall Gecko Score (beha…`
- `latest_findings`: `Latest notable results detected in the Gecko Tests and price data (fixed rules, numbers and quotes from stored results).`
- `search`: `Search BenchGecko models and Gecko Tests. Returns ids for fetch.`
- `search_models`: `Find AI models in the BenchGecko catalog by name, slug or lab. Returns slugs to use with get_model, cheapest_provider and compare_models, w…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://benchgecko.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
