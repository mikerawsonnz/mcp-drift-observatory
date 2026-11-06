# prices.brainy.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/prices.brainy.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://prices.brainy.ae/mcp/v2` | 26 | [`d04ccd90cf77`](9443ab886276db8be110.json) | 2026-11-06 |
| `https://prices.brainy.ae/mcp` | 19 | [`23e8b3cbe91c`](f6d1febd0eda9114989e.json) | 2026-11-02 |

## Tools at `https://prices.brainy.ae/mcp/v2`

- `commute_cost`: `Monthly/annual car commute cost (fuel+Salik), or published area routes. No parking.`
- `costs_by_area`: `Dubai areas ranked by monthly cost: rent, fees, bills (+school). Not full budgets.`
- `costs_by_emirate`: `Compare emirates: rent, utilities, schools. Non-Dubai rent unknown.`
- `data_sources`: `Where each number comes from: publishers, licences, dates, paused sources.`
- `dewa`: `DEWA electricity/water: tariff slabs, or bill estimate from kwh (+water, VAT, fee).`
- `end_of_service_gratuity`: `UAE private-sector end-of-service gratuity estimate (Decree-Law 33/2021 art. 51): basic wage + dates → amount or range; not legal advice.`
- `fixed_monthly_costs`: `Monthly fixed costs for a household profile, with assumptions. Not a full budget.`
- `free_zone_companies`: `Free zone company setup: package prices, annual/monthly cost, visas.`
- `fuel_prices`: `UAE petrol/diesel prices this month and last, change, 50/70 L tank cost, history.`
- `fx_rates`: `Dated CBUAE AED exchange rates. Not bank quotes.`
- `grocery_compare_list`: `Cheapest store for a list: subtotals, delivery fees, minimums. items: ["milk"]. Observed + labelled estimates.`
- `grocery_products`: `Dubai supermarket prices: per-store pack/unit offers, dates, history. Give query (product name), e.g. milk, or product_id. Not MOET.`
- `grocery_stores`: `Grocery stores: delivery fees, free-delivery thresholds, minimum orders.`
- `health_insurance`: `Dubai health insurance rules: who pays, basic plan band/benefits, fines. Not quotes.`
- `housing_rents`: `Registered Dubai rent: annual/monthly medians, contract counts. zone or q: JVC. Not listings.`
- `housing_sales`: `Sale prices by Dubai area: ready/off-plan registered medians. Not listings.`
- `labour_calculator`: `UAE labour law estimates (Decree-Law 33/2021): overtime pay, annual leave, final settlement. Not legal advice.`
- `ministry_shop_prices`: `MOET-published Dubai shop prices. category: bread or chain_id/product_id. Not online offers.`
- `mobile_internet_plans`: `UAE mobile and home internet plans: VAT-inclusive price, data, contract.`
- `move_to_dubai`: `Move to Dubai? Home vs Dubai net pay, taxes, FX, costs, savings. No country: models. Owner: household=business_owner + profit. Not tax advi…`
- `residence_visas`: `UAE residence visas by route: payer, requirements, fees, medical/insurance bands.`
- `schools`: `Dubai school fees: KHDA tuition by grade/year, bus fees, distance. q: school name; near: zone (JVC). Year ≠ Grade; uniforms paused.`
- `shopper_price_reports`: `Community price reports by product/store, with date and promos.`
- `start_here`: `Tool selection help: examples and citations.`
- `tax_savings_by_country`: `Tax saved by moving to Dubai, per country, typical pay. Not tax advice.`
- `transport_fares`: `Taxi fare estimate, or metro/bus fares, parking and toll tariffs. Not app quotes.`

## Tools at `https://prices.brainy.ae/mcp`

- `compare_areas_cost_of_living`: `Rank Dubai communities by estimated monthly cost of living: median registered rent + Dubai Municipality housing fee + DEWA (official slabs,…`
- `compare_grocery_list`: `Compare the total cost of a grocery list across Dubai supermarkets. Uses observed catalogue prices and published delivery rules; unknown de…`
- `estimate_commute_cost`: `Monthly cost of a car commute in Dubai with this month's official fuel price and Salik tolls (same formula as the website: days per month =…`
- `estimate_move_to_dubai`: `Salary after tax at home vs in Dubai — Nothing deducted (model assumption; Cabinet Decision 49 of 2023) — or with household="business_owner…`
- `find_price_online`: `PAUSED: live online price references are switched off while a legal review is under way; calls return an error. Find indicative online pric…`
- `get_cost_of_living`: `Fixed monthly costs in Dubai this month for a single person (studio), a couple (1-bedroom) and a family of four (2-bedroom, two children in…`
- `get_dewa_tariff`: `DEWA electricity and water slab tariff with this month's fuel surcharge and VAT, plus a monthly bill estimate for your kWh and water use (i…`
- `get_electronics_prices`: `Prices of popular phones, laptops, tablets, consoles, headphones, watches and TVs at Dubai stores (Sharaf DG, Jumbo, Amazon.ae, noon, Carre…`
- `get_fuel_prices`: `UAE petrol and diesel prices for the current month (AED per litre, official monthly announcement), change vs last month, full-tank cost and…`
- `get_health_insurance`: `Health insurance rules in Dubai from official texts, each with its article and source: who must pay (employer or sponsor), the minimum cove…`
- `get_mobile_internet_plans`: `Dubai mobile postpaid and home internet plans (Virgin Mobile, du, e&) with price per month including 5% VAT, data, minutes, contract and pr…`
- `get_product`: `Get a catalogue product, observed store offers and product history where available. Basket-total history is never presented as product hist…`
- `get_rent_prices`: `Median annual rent by community, property type and bedrooms from registered Ejari contracts (Dubai Land Department open data, last 12 month…`
- `get_school_fees`: `Annual tuition of Dubai private schools as published by KHDA (by grade, area, curriculum, inspection rating), with the school bus fee by zo…`
- `get_school_uniforms`: `Official school uniform items and prices for a Dubai/UAE school (supplier catalogue, item by item), plus KHDA tuition and school bus fees w…`
- `get_taxi_fares`: `Dubai taxi fares as published by Dubai Taxi Company (DTC): street-hail and booked (e-hail) starting fares by time of day, rate per km, wait…`
- `get_visa_and_company_costs`: `Official government fees to move to Dubai by residence route (job, family, golden, remote work, freelance, investor): work permit, entry pe…`
- `list_stores`: `List Dubai stores and their published delivery rules, minimum orders, source URLs and verification dates. Unknown or expired delivery rules…`
- `search_products`: `Search the observed Dubai grocery catalogue by name, brand or identifier. Returns exact/equivalent matches and dated offers in AED. This do…`

## Changes

- 2026-11-06: [schema changed](../../deltas/2026-11-06/9443ab886276db8be110.json): `17 field(s) changed`
- 2026-11-03: [description changed](../../deltas/2026-11-03/9443ab886276db8be110.json): `7 field(s) changed`
- 2026-11-02: [description changed](../../deltas/2026-11-02/f6d1febd0eda9114989e.json): `1 field(s) changed`
- 2026-10-31: [schema changed](../../deltas/2026-10-31/f6d1febd0eda9114989e.json): `245 field(s) changed`
- 2026-10-31: [schema changed](../../deltas/2026-10-31/9443ab886276db8be110.json): `414 field(s) changed`
- 2026-10-22: [count changed, tool removed](../../deltas/2026-10-22/f6d1febd0eda9114989e.json): `1 tool(s) removed`
- 2026-10-22: [count changed, tool removed](../../deltas/2026-10-22/9443ab886276db8be110.json): `1 tool(s) removed`
- 2026-10-15: [count changed, tool added](../../deltas/2026-10-15/9443ab886276db8be110.json): `1 tool(s) added`
- 2026-10-14: [count changed, schema changed, tool added](../../deltas/2026-10-14/9443ab886276db8be110.json): `1 tool(s) added; 25 field(s) changed`
- 2026-10-13: [annotation changed, count changed, description changed, tool added, tool removed](../../deltas/2026-10-13/9443ab886276db8be110.json): `2 tool(s) added; 1 tool(s) removed; 46 field(s) changed`
- 2026-10-07: [description changed, schema changed](../../deltas/2026-10-07/9443ab886276db8be110.json): `7087 field(s) changed`
- 2026-10-07: [description changed, schema changed](../../deltas/2026-10-07/f6d1febd0eda9114989e.json): `610 field(s) changed`
- 2026-10-05: [schema changed](../../deltas/2026-10-05/f6d1febd0eda9114989e.json): `31 field(s) changed`
- 2026-10-04: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-04/f6d1febd0eda9114989e.json): `2 tool(s) added; 40 field(s) changed`
- 2026-10-03: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-03/f6d1febd0eda9114989e.json): `13 tool(s) added; 9 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://prices.brainy.ae/mcp/v2"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
