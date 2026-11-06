# agenlify.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agenlify.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agenlify.ai/mcp` | 3 | [`af24171defa0`](af8840ee5a1320cc5990.json) | 2026-10-14 |

## Tools at `https://agenlify.ai/mcp`

- `get_agent`: `Get a catalog product by exact slug, including inputs, outputs, setup steps, limitations, human review requirements, pricing review dates,…`
- `list_tasks`: `List Agenlify task IDs, preparation checklists, expected outputs and review requirements. Each listed task has at least three catalog candi…`
- `search_agents`: `Search the public Agenlify catalog by English or Chinese task, product name or official domain. Filter by pricing, setup, category, task an…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agenlify.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
