# mcp.discond.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.discond.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.discond.ae/mcp` | 9 | [`af4d18a0e527`](cd7db03de9f0ecc82710.json) | 2026-11-26 |

## Tools at `https://mcp.discond.ae/mcp`

- `discond_autocomplete_businesses`: `Typo-tolerant autocomplete of UAE merchant names on Discond. Returns matching merchant ids and names for partial or misspelled input.`
- `discond_find_discounts`: `Search UAE merchants with live discounts on Discond by free text, place (emirate or area such as "Dubai Marina"), coordinates, discount pro…`
- `discond_find_venues`: `Find UAE restaurants, cafés and other venues near an area or landmark (e.g. "Burj Khalifa", "Dubai Marina", "Yas Island") that fit a cuisin…`
- `discond_get_business`: `Get one Discond merchant by id: name, a short description when we have one, categories, providers, link and its branches. Pass the user's l…`
- `discond_get_offer`: `Get one Discond offer by id: headline, terms, validity and redeem links. Requires the user to be signed in to Discond.`
- `discond_list_categories`: `List Discond merchant categories with ids, optionally filtered by name.`
- `discond_list_offers`: `List live Discond offers, filtered by merchant, branch, provider, category, validity or online-only, sorted by newest, expiring or biggest…`
- `discond_list_providers`: `List the discount providers Discond covers (for example Fazaa, The Entertainer, Talabat) with ids and offer counts, optionally filtered by…`
- `discond_resolve_place`: `Resolve a UAE place name to Discond place ids (emirate, community, settlement) or to a known area. A known area or landmark (Burj Khalifa,…`

## Changes

- 2026-11-26: [schema changed](../../deltas/2026-11-26/cd7db03de9f0ecc82710.json): `4 field(s) changed`
- 2026-11-20: [description changed, schema changed](../../deltas/2026-11-20/cd7db03de9f0ecc82710.json): `10 field(s) changed`
- 2026-11-17: [schema changed](../../deltas/2026-11-17/cd7db03de9f0ecc82710.json): `35 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-11-16: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-16/cd7db03de9f0ecc82710.json): `1 tool(s) added; 3 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.discond.ae/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
