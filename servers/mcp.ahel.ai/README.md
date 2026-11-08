# mcp.ahel.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.ahel.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.ahel.ai` | 11 | [`9bad498c660a`](f81cefdfba92e36c524a.json) | 2026-11-08 |

## Tools at `https://mcp.ahel.ai`

- `balance`: `The workspace's prepaid balance in USD, what runs in flight hold, what settled runs used today and this month (shown to the Owner), any dai…`
- `capability_inspect`: `Read one task or provider tool from Ahel's catalog by its id: its exact inputs (Ahel's own contract, or the published reference input when…`
- `capability_run_status`: `Without execution_id: the paid data capabilities this workspace can run, each with its providers and exact prices. With execution_id: that…`
- `capability_search`: `Search Ahel's catalog of data tasks and provider tools by words, a task id or a tool id: company and people enrichment, SEO, social, ads, e…`
- `catalog_request`: `Ask Ahel to add a data task or provider tool the catalog does not have yet: call it when capability_search answers verdict none and none of…`
- `feedback`: `Rate one run or one catalog request of this workspace good or bad, or, with no id, report anything about Ahel: confusing results or charges…`
- `get_started`: `How to start with Ahel: call this when the person asks what Ahel is, what it can do or how to begin. Returns what Ahel is, how the prepaid…`
- `my_tools`: `This team's own tools: the APIs and MCP servers the team added at ahel.ai/app/tools. Without tool, lists each one with its tools, their inp…`
- `review`: `Rate how useful one finished run of this workspace was, after you have used its result: useful, partly, not_useful, or not_sure when you ca…`
- `run_batch`: `Run one task over many inputs in one call: for repeated runs of the same task, one round trip rather than one per run. Priced the same per…`
- `run_capability`: `Run one paid data capability (company data, people and contact data and the like) through Ahel's provider execution: it is quoted, the exac…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.ahel.ai"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
