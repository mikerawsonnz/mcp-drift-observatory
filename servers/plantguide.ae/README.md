# plantguide.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/plantguide.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://plantguide.ae/mcp` | 15 | [`cfa6956257a3`](d68ae98758c08444a69b.json) | 2026-10-30 |

## Tools at `https://plantguide.ae/mcp`

- `build_designer_link`: `A link that opens our free 3D garden planner with the given plants already in the plant list, so the person can plan a layout or send the l…`
- `estimate_garden_care_price`: `Monthly Garden Care price (AED, excluding 5% VAT) for a Dubai villa from garden area, lawn type, pool size, complexity and number of trees,…`
- `get_contact_link`: `A WhatsApp click-to-chat link with a pre-filled message (topic, plants, community and notes) for when the person wants a quote, a visit or…`
- `get_dubai_climate`: `Dubai's monthly average high and low temperatures and rainfall (WMO 1991–2020 normals), the planting season and summer work-ban months, and…`
- `get_garden_style`: `The full guide to one garden style: why choose it, the mood, its anatomy, upkeep (weekly, monthly, seasonal), water, who it suits and doesn…`
- `get_guide`: `One guide in full, as Markdown, with its FAQ and sources.`
- `get_indoor_plant_guide`: `The starting point for anything about houseplants and indoor plants in Dubai: choosing by light (low, medium, bright indirect, direct sun),…`
- `get_indoor_style`: `The full guide to one indoor plant style for Dubai homes: mood and palette, key plants with their light and pet safety, pots and materials,…`
- `get_kitchen_garden_guide`: `How to grow vegetables, herbs and fruit at home in Dubai: the sowing and harvest calendar, raised beds vs pots vs a fruit-tree corner, a st…`
- `get_plant`: `Everything about one plant in Dubai: ratings, size, sun and water, seasonal calendar, watering in summer and winter, soil, feeding, pruning…`
- `get_planting_calendar`: `Sow, plant, flower, harvest, prune and feed months for a set of plants (by slug, category or group), as a 12-month grid. Use it to compare…`
- `list_garden_styles`: `The garden styles we design in Dubai (tropical, manicured, luxury, desert modern) with mood, upkeep effort, water use, build cost per m² an…`
- `search_guides`: `Find our practical guides (planting calendar, summer watering, lawn grasses, indoor plants, costs, approvals and more) by keyword, topic or…`
- `search_plants`: `Search and filter the library of plants rated for Dubai's heat, salt, drought and shade: by name (English, botanical, Arabic or a local nam…`
- `what_to_plant`: `What to sow and plant in Dubai in a given month or season, plus what is flowering, fruiting or ready to harvest, the month's verdict, tips,…`

## Changes

- 2026-10-30: [schema changed](../../deltas/2026-10-30/d68ae98758c08444a69b.json): `12 field(s) changed`
- 2026-10-12: [description changed, schema changed](../../deltas/2026-10-12/d68ae98758c08444a69b.json): `4 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://plantguide.ae/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
