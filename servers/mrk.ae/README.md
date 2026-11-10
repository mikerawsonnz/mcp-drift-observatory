# mrk.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mrk.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mrk.ae/api/mcp` | 22 | [`3ea43485a7c0`](bb43c026bcc1ebed4e48.json) | 2026-11-10 |

## Tools at `https://mrk.ae/api/mcp`

- `ask`: `Answer a free-text Dubai property question (e.g. '2 bed off-plan in Dubai Hills under 3M handover 2027'). Parses community, developer, bedr…`
- `calculate_dld_buying_costs`: `Calculate Dubai Land Department transfer fees and total buying costs for a Dubai property purchase.`
- `calculate_mortgage`: `Monthly repayment, total interest and loan-to-value for a repayment mortgage. Pure arithmetic on the rate you supply; UAE Central Bank base…`
- `calculate_purchase_costs`: `Itemised one-off costs of buying in Dubai using MRK's verified fee schedule: DLD 4% transfer fee, DLD admin fee, title deed, registration t…`
- `check_golden_visa_eligibility`: `Check if a Dubai property investment qualifies for UAE Golden Visa (10-year residency). Minimum threshold is AED 2 million.`
- `compare_projects`: `Side-by-side comparison of 2 to 5 projects by slug: developer, community, stage, handover, starting price, unit types, payment plan.`
- `get_community`: `Community stats: project count, off-plan/ready split, developers, starting-price bands (lowest/median/highest) and top projects.`
- `get_developer`: `Developer profile: project count, off-plan/ready split, communities, starting-price statistics and its top projects.`
- `get_dubai_community_facts`: `Get key facts about a Dubai community including price per sqft, rental yield and Golden Visa qualifying status.`
- `get_insight`: `Full insight article by slug: summary, key numbers with sources, body sections, FAQs and source list.`
- `get_listing`: `Full details of one live MRK sale listing by web slug or reference.`
- `get_project`: `Full facts for one project by slug or exact name: developer, community, status, handover, starting prices by unit type, payment plan, highl…`
- `get_rent_cap_increase`: `Calculate the maximum legal rent increase in Dubai per RERA Decree 43/2013 rent cap tiers based on how far current rent is below market ave…`
- `golden_visa_eligibility`: `Indicative check against the UAE 10-year Golden Visa real-estate route (property value of at least AED 2 million). Returns shortfall and co…`
- `list_communities`: `List Dubai communities with project counts and lowest starting price, optionally filtered by name text. Sorted by project count.`
- `list_developers`: `List Dubai developers with project counts (off-plan vs ready), optionally filtered by name text. Sorted by project count.`
- `rental_yield_estimate`: `ESTIMATE of gross and net rental yield from a price and an annual rent you supply (plus optional service charge and other annual costs). MR…`
- `search_glossary`: `Search the MRK Dubai real estate glossary for a term definition. Returns matching terms with definitions.`
- `search_insights`: `Search MRK's sourced Dubai market insights (original commentary with linked sources). Filter by text and category.`
- `search_listings`: `Search MRK Real Estate's live sale listings (from the MRK CRM, refreshed every 5 minutes). Filter by text, location, type, price and bedroo…`
- `search_projects`: `Search ~2,400 Dubai residential projects (DLD-registered plus MRK-researched new launches). Filter by community, developer, stage, handover…`
- `submit_enquiry`: `Send a buyer/seller enquiry to MRK Real Estate's advisory team on the user's behalf. Only call with the user's explicit consent. Requires n…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mrk.ae/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
