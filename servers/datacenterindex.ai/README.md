# datacenterindex.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/datacenterindex.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://datacenterindex.ai/mcp` | 8 | [`473a630e0094`](49111276a36144278889.json) | 2026-09-23 |

## Tools at `https://datacenterindex.ai/mcp`

- `get_company`: `One public company by ticker: description, data-center exposure, market cap, and the tracked projects it is linked to.`
- `get_market`: `One US state market: summary description, counts, the tracked projects, and the public companies exposed to it.`
- `get_movers`: `Biggest day and week stock moves across the tracked universe (latest close).`
- `get_project`: `One tracked project by slug (the last path segment of a datacenterindex.ai/projects/... URL), with its linked public companies.`
- `list_companies`: `Public companies in the tracked supply-chain universe with sector, data-center revenue exposure and project count.`
- `list_markets`: `Every US state market with tracked projects: counts by status, pipeline MW, grid operator, page URL.`
- `recent_changes`: `What changed in the tracker recently: new projects, status changes, capacity revisions. The single source for "what is new".`
- `search_projects`: `Search tracked data center projects. Filter by free-text query (name, developer, tenant, city), US state code, status, developer, or minimu…`

## Changes

- 2026-09-23: [schema changed](../../deltas/2026-09-23/49111276a36144278889.json): `2 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://datacenterindex.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
