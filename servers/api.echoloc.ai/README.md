# api.echoloc.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.echoloc.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.echoloc.ai/mcp` | 3 | [`7a608b2a5581`](e0a8087e9b82f9cc438d.json) | 2026-09-30 |

## Tools at `https://api.echoloc.ai/mcp`

- `get_company_by_domain`: `Resolve a company domain (e.g. 'walgreens.com') to its full profile: firmographics, hiring stats, and the technology stack with adoption co…`
- `list_technologies`: `Catalog of all technologies in the dataset with per-technology company counts. sort='count' (most used first) or 'name'.`
- `search_companies_by_technologies`: `Find companies using the given technologies, ranked by usage. Names are case-insensitive ('snowflake' == 'Snowflake'); 10,000+ technologies…`

## Changes

- 2026-09-30: [description changed, schema changed](../../deltas/2026-09-30/e0a8087e9b82f9cc438d.json): `2 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.echoloc.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
