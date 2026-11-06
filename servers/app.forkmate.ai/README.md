# app.forkmate.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.forkmate.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.forkmate.ai/mcp` | 11 | [`cdc28be7edd8`](a80c56f4a3b87148f0d9.json) | 2026-10-04 |

## Tools at `https://app.forkmate.ai/mcp`

- `delete_meal`: `Delete one food from a diary entry (by 'item_index'), or the whole entry (without it). The entry is identified by 'id' and 'local_date'. De…`
- `get_day`: `Read the user's food diary for one day: its entries, each listed with its 'id' and each food with its item_index, quantity and macros, and…`
- `get_preferences`: `Read the user's food profile: diet style, allergies (a structured list of the major US allergens), foods they like, foods they dislike, and…`
- `get_range`: `Read the user's food diary across a date range, with per-day calorie/macro totals and each entry listed with its 'id'. All calorie and macr…`
- `get_usual_foods`: `Read what the user usually and recently eats. 'usual' lists their most-logged foods, most frequent first, each with how many times it was l…`
- `log_meal`: `Add a meal to the user's food diary: one or more food items, each with an optional quantity and macros, plus an optional meal label, date,…`
- `lookup_barcode`: `Look up a packaged food by its UPC/EAN barcode in Open Food Facts. Returns macros per 100 g, a 'source' label ('Open Food Facts'), and, whe…`
- `search_foods`: `Search USDA FoodData Central, Open Food Facts and Forkmate's curated restaurant menus for a named food. Returns up to 5 candidates, each wi…`
- `update_meal`: `Correct a food already in the user's diary — its name, quantity, macros, caffeine or fluid — or change an entry's meal label or note. The e…`
- `update_preferences`: `Edit the user's food profile: add or remove foods they like or dislike, add or remove allergies from the major US allergen list, or set the…`
- `whoami`: `Diagnostic: confirms that this connection is signed in to a Forkmate account. Returns no account id, email or other identifier.`

## Changes

- 2026-10-04: [description changed, schema changed](../../deltas/2026-10-04/a80c56f4a3b87148f0d9.json): `4 field(s) changed`
- 2026-10-02: [annotation changed, count changed, description changed, schema changed, tool added, tool removed](../../deltas/2026-10-02/a80c56f4a3b87148f0d9.json): `2 tool(s) added; 3 tool(s) removed; 139 field(s) changed; signals: length_more_than_doubled`
- 2026-10-01: [annotation changed, schema changed](../../deltas/2026-10-01/a80c56f4a3b87148f0d9.json): `415 field(s) changed`
- 2026-09-30: [description changed, schema changed](../../deltas/2026-09-30/a80c56f4a3b87148f0d9.json): `21 field(s) changed`
- 2026-09-24: [description changed](../../deltas/2026-09-24/a80c56f4a3b87148f0d9.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.forkmate.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
