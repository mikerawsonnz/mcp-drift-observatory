# api.epinu.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.epinu.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.epinu.ai/api/agent/mcp` | 5 | [`8a352dc9a312`](5f26c2692199a1c07bdb.json) | 2026-08-20 |

## Tools at `https://api.epinu.ai/api/agent/mcp`

- `fetch`: `Fetch the full document for one search result by its opaque id (project:<uuid> or listing:<uuid>). Returns { id, title, text, url, metadata…`
- `getting_started`: `Start here: platform overview, the proposal/approval operating model, auth rules, common flows, and agent etiquette. Static content — requi…`
- `marketplace_listings_search`: `Search the Epinu marketplace for equipment, services, and assets. Returns summaries only; call marketplace_listing_get for detailed packets.`
- `projects_search`: `Search Epinu real-asset projects. Returns bounded summaries only; call projects_get_deep_dive for detailed packets. Results include public…`
- `search`: `Unified read-only search across public Epinu projects and marketplace listings. Returns { id, title, url } results; call fetch with a retur…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.epinu.ai/api/agent/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
