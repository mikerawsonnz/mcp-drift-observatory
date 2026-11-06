# tandem.ac: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/tandem.ac.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://tandem.ac/mcp` | 13 | [`73dd9c8626a0`](1a1978d681b968f5e968.json) | 2026-08-20 |

## Tools at `https://tandem.ac/mcp`

- `answer_how_to`: `Answer how to install or use Tandem, build workflows, or use the SDKs by synthesizing relevant published docs.`
- `compare_doc_page_refresh`: `Force-refresh a docs page and return before/after hashes so page content changes can be proven.`
- `compare_docs_index_refresh`: `Force-refresh the docs indexes and return before/after hashes so content changes can be proven.`
- `get_doc`: `Fetch and normalize a published Tandem docs page by path or URL.`
- `get_docs_cache_status`: `Inspect the current docs cache state for index sources and warmed pages.`
- `get_start_path`: `Recommend the best Tandem docs starting path for a desktop user, server admin, or developer.`
- `get_tandem_guide`: `Return a structured Tandem learning guide for install-engine, python-sdk, typescript-sdk, build-workflows, or headless-deploy.`
- `invalidate_docs_cache`: `Invalidate docs cache entries for index data, all pages, or a specific page path.`
- `recommend_next_docs`: `Recommend the next Tandem docs to read after a current page, optionally biased toward a goal.`
- `refresh_doc_page`: `Force-refresh a docs page and report whether content came from the network, cache, or stale fallback.`
- `refresh_docs_index`: `Force-refresh docs indexes and report whether data came from the network, cache, or stale fallback.`
- `search_docs`: `Search the published Tandem docs index for relevant pages.`
- `warmup_docs_cache`: `Refresh the docs index and preload the most important Tandem docs pages into cache.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://tandem.ac/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
