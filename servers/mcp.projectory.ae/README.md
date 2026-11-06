# mcp.projectory.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.projectory.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.projectory.ae/mcp` | 6 | [`09d964fdb296`](fc2bf3f491231659286d.json) | 2026-11-03 |

## Tools at `https://mcp.projectory.ae/mcp`

- `fetch`: `Fetch one development's detail using a known ID, slug or Projectory URL; no prior search or facet lookup is needed. Returns development-wid…`
- `list_project_facets`: `Explore all exact values for 'emirate', 'area', 'developer', 'propertyType', 'availability' and 'sort', plus boolean flags 'newLaunch' and…`
- `list_research_reports`: `List citable Projectory Research reports, newest first. Reports analyse registered residential sales from Dubai Land Department (DLD) and A…`
- `search`: `Find published off-plan UAE developments by project name or slug text, combined with exact structured filters. Returns shortlist facts and…`
- `search_transactions`: `Search canonical residential sale registrations in one required market: Dubai or Abu Dhabi. Whole area, project and building names ignore A…`
- `suggest_project_terms`: `Resolve partial emirate, area, developer or property-type text, such as "marina" or "sobha", into exact filter slugs for 'search'. Does not…`

## Changes

- 2026-11-03: [count changed, tool added](../../deltas/2026-11-03/fc2bf3f491231659286d.json): `1 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.projectory.ae/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
