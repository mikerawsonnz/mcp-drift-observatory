# law.agentlookups.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/law.agentlookups.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://law.agentlookups.ai/mcp` | 4 | [`085d98c5e2d0`](ca5a5fcdc8fec39a1452.json) | 2026-10-28 |

## Tools at `https://law.agentlookups.ai/mcp`

- `law_coverage`: `Per-source coverage: what we host, section counts, current-through or vintage, last_verified, and a stale flag for any source the recurring…`
- `law_for_location`: `Resolve an address or lat/lon to its full jurisdiction stack: federal, state, county, place, each with its code sources (name, publisher, o…`
- `law_get_section`: `Fetch full verbatim text by id or citation, or pass references for a batch of up to 10. Each batch item has its own result/error. Includes…`
- `law_search`: `Search original law by topic, question, or citation. Exact citations resolve directly. Scoped by jurisdiction or source ids (e.g. us, us-tx…`

## Changes

- 2026-10-28: [description changed, schema changed](../../deltas/2026-10-28/ca5a5fcdc8fec39a1452.json): `5 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://law.agentlookups.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
