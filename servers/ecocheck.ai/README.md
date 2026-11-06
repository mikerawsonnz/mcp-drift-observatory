# ecocheck.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/ecocheck.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://ecocheck.ai/mcp` | 14 | [`e004d8935f9e`](804953eaaa3f0cf8f976.json) | 2026-10-11 |

## Tools at `https://ecocheck.ai/mcp`

- `about_ecocheck`: `What EcoCheck is (company, product, services) with links to its pricing page, case studies and contact page.`
- `calculate_ghg_inventory`: `GHG inventory from activity data, reported by ISO 14064-1 category (1-6), GHG Protocol scope and gas: fuels (IPCC 2006 tier-1 defaults; lit…`
- `cbam_default_value`: `EU CBAM default value (tCO2e per tonne) of a CN8 code for a country of production, from Implementing Regulation (EU) 2025/2621 as corrected…`
- `cbam_scope_check`: `EU CBAM: is a product (CN code) in scope, which aggregated goods category, are indirect emissions counted, and its EU default value for the…`
- `check_ghg_inventory_obligation`: `Check whether a Vietnamese facility must do a mandatory greenhouse-gas (GHG) inventory under Decree 06/2022 (amended by 119/2025) and the 2…`
- `estimate_cbam_cost`: `Indicative CBAM certificate cost for the EU importer: embedded emissions (default value with mark-up, or the producer's actual SEE) minus t…`
- `get_article`: `Get one EcoCheck article as Markdown by numeric id or slug (from list_articles / search_ecocheck).`
- `get_ghg_regulations`: `Key verified facts for Vietnam GHG compliance in 2026: Decision 42/2026 facility list (2,441 facilities), reporting deadline 31/3/2027, pil…`
- `get_pricing`: `EcoCheck software plans (Basic free, Pro 4,950,000 VND/month, Pro+ 10,950,000 VND/month, Advanced custom) and where to find inventory-servi…`
- `ghg_emission_factors`: `Built-in default factors used by calculate_ghg_inventory: fuels (NCV, CO2/CH4/N2O, density), refrigerant GWPs (AR5 / AR6), GWP sets. Cite t…`
- `iso14064_guide`: `Practical guidance for an ISO 14064-1 organization inventory (paraphrased, not the standard text): categories and boundaries with the Scope…`
- `list_articles`: `List EcoCheck articles (Vietnamese), newest first, optionally filtered by keyword.`
- `list_services`: `List EcoCheck services: GHG inventory service, inventory software platform, CBAM reporting, ESG reporting, free obligation lookup tool, Aca…`
- `search_ecocheck`: `Search EcoCheck services, regulations and Vietnamese articles on GHG inventory, Scope 1/2/3, CBAM, carbon credits and ESG. Returns ranked m…`

## Changes

- 2026-10-11: [schema changed](../../deltas/2026-10-11/804953eaaa3f0cf8f976.json): `7 field(s) changed; signals: length_more_than_doubled`
- 2026-10-10: [annotation changed, description changed, field changed](../../deltas/2026-10-10/804953eaaa3f0cf8f976.json): `34 field(s) changed`
- 2026-10-09: [count changed, tool added](../../deltas/2026-10-09/804953eaaa3f0cf8f976.json): `6 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://ecocheck.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
