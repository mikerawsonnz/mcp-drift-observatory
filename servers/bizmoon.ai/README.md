# bizmoon.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/bizmoon.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://bizmoon.ai/api/mcp` | 5 | [`4dcea0ac454a`](60513f782b423d70a731.json) | 2026-09-19 |

## Tools at `https://bizmoon.ai/api/mcp`

- `changes_since`: `Everything published since a given date, optionally for one jurisdiction, newest first. Designed for scheduled or recurring agents: store t…`
- `get_regulatory_change`: `Fetch one regulatory document by id: title, jurisdiction, agencies, category, published and effective dates, AI summary, full description,…`
- `list_jurisdictions`: `List every jurisdiction and official register Bizmoon monitors, with the most recent publication date, and when the source was last checked…`
- `search_funding_programs`: `Search federal and state grant and incentive programs (grants.gov plus state economic development agencies) by keyword, jurisdiction, agenc…`
- `search_regulatory_changes`: `Search US federal and state regulatory documents ingested from official registers, with AI summaries, agencies, effective dates, and source…`

## Changes

- 2026-09-19: [annotation changed, description changed, schema changed](../../deltas/2026-09-19/60513f782b423d70a731.json): `13 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://bizmoon.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
