# mcp.gondola.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.gondola.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.gondola.ai/mcp` | 44 | [`efe5900f4ed5`](9dc511da618e354e45d7.json) | 2026-09-26 |

## Tools at `https://mcp.gondola.ai/mcp`

- `book_flight`: `Book a prepared flight only after the traveler explicitly confirms the exact current quote, total, currency, and consent version. Use the h…`
- `book_hotel`: `Book a hotel room using a rate from get_hotel_rates. Requires guest details and a saved payment method. Use get_payment_methods to find the…`
- `book_vehicle`: `Book a rental vehicle from a search result. Requires a Gondola account and a saved payment method (use get_payment_methods to find the paym…`
- `cancel_flight_booking`: `Preview flight cancellation first with confirm=false or omitted. Show the returned itinerary cancellation scope and exact terms before aski…`
- `cancel_vehicle_booking`: `Cancel an existing vehicle booking by its Gondola booking ID. Use this when a user wants to cancel a rental they previously booked.`
- `compare_rates`: `Compare current canonical cash vs points rates side-by-side for one or more hotels. Use this whenever the user is making a cash-vs-points d…`
- `create_rate_alert`: `Create a rate alert to monitor a hotel for price drops. The user will be notified by email when the rate drops. Optionally specify dates, o…`
- `credit_card_coverage`: `Look up rental car CDW/LDW (collision damage waiver / loss damage waiver) coverage provided by a credit card. Useful before booking — tells…`
- `delete_rate_alert`: `Delete a rate alert to stop monitoring a hotel for price drops.`
- `diagnose_rates`: `Diagnose rate availability and per-supplier statuses for a specific hotel. Use this when a power user asks why certain rates aren't showing…`
- `get_booking`: `Get details for a hotel booking made through Gondola, using the Gondola booking ID shown as "Gondola booking" by get_upcoming_trips and get…`
- `get_booking_link`: `Get a booking link for a hotel on Gondola. Use this when a user wants to book a specific hotel. Returns a URL to the hotel's booking page w…`
- `get_favorite_hotels`: `Get the hotels the user has saved as favorites in Gondola, newest first. Use this when the user asks about their favorite or saved hotels,…`
- `get_flight_booking`: `Get the current owner-scoped state of a Gondola flight booking, including booking, payment, ticketing, action-required, cancellation, ticke…`
- `get_flight_credits`: `Get the user's active airline flight credits, eCredits, travel funds, vouchers, and travel-bank balances. Returns the airline, remaining us…`
- `get_flight_points`: `Collect award (miles/points) pricing for a flight search that reported pending_sources. Call this after search_flights when you set points:…`
- `get_free_night_credits`: `Get the user's free night certificates — the award nights earned from credit cards and elite status, such as a Marriott Free Night Award, a…`
- `get_hotel_details`: `Get stored property information for a specific hotel: address, chain and brand, property type, star and guest ratings, all-inclusive and ad…`
- `get_hotel_rates`: `Get live room rates for one hotel and stay window. Rooms are grouped by type (up to 12 shown) with up to three rates each: the cheapest non…`
- `get_hotel_reviews`: `Get guest reviews for a specific hotel. Use this to help a user understand what other guests thought about a property — common complaints,…`
- `get_hotel_stats`: `Get pricing percentile context for a specific hotel. Returns where the current rate falls relative to the property's typical pricing (e.g.…`
- `get_loyalty_accounts`: `Get the user's loyalty program memberships and current point balances. Use this to personalize recommendations (e.g. "with 120k Bonvoy poin…`
- `get_multi_night_rates`: `Get cached, partial rate observations for a hotel over a flexible date range. Use this for seasonality shape and to shortlist candidate che…`
- `get_past_trips`: `Get the user's past hotel stays and flights. Use this to answer travel-history questions and make recommendations grounded in behavior (e.g…`
- `get_payment_methods`: `List the user's saved payment methods for booking. Returns saved credit/debit cards with their payment IDs, needed for the book_hotel tool.`
- `get_rate_alerts`: `Get all active rate alerts for the current user. Returns which hotels the user is monitoring for price drops.`
- `get_similar_hotels`: `Find hotels similar to a given hotel. Use this for branching exploration after a search (e.g. user likes the Park Hyatt Tokyo but wants a c…`
- `get_suggested_searches`: `Get personalized travel suggestions and trip inspiration for the current user. Returns curated hotel recommendations grounded in the user's…`
- `get_suite_upgrade_credits`: `Get the user's active suite upgrade awards and certificates across loyalty programs. Returns the program, award type, remaining count, and…`
- `get_travel_profiles`: `Get the user's saved travel profiles — guest name, email, and phone presets. Each profile has a selectable ID you can pass to book_hotel as…`
- `get_traveler_context`: `Get the user's saved travel context: loyalty programs and elite tiers, home airport, preferred airlines and cabin, preferred hotel chains,…`
- `get_upcoming_trips`: `Get the user's upcoming hotel, flight, and rental car reservations. Use this to ground recommendations in real plans (e.g. "your Tokyo trip…`
- `get_vehicle_booking`: `Get details for a specific vehicle booking by its Gondola booking ID. Returns vendor, pickup/dropoff locations and times, vehicle class, ra…`
- `get_vehicle_booking_coverage`: `Get the rental car CDW/LDW coverage that was stored at booking time for a specific vehicle booking. Use this after a booking to remind the…`
- `get_vehicle_booking_link`: `Get a Gondola.ai deep link for a specific vehicle from search results. Use this to share a booking page URL the user can complete on the we…`
- `get_vehicle_details`: `Get detailed information about a specific rental vehicle option. Use this after search_vehicles to get extras, insurance options, charges,…`
- `optimize_loyalty_portfolio`: `Analyze the user's entire loyalty portfolio and surface the highest-value actions: points expiring soon (ranked by value at risk), the best…`
- `predict_price`: `Predict whether the current rate at a hotel is a good deal based on historical price trends. Use this when the user is debating booking now…`
- `prepare_flight_booking`: `Prepare a flight for booking from a signed selection_token that comes only from an eligible search_flights row. Search re-shops the selecte…`
- `search_events`: `Search for live events by artist, team, show, or event name. Returns factual event discovery details in provider order, including dates, ve…`
- `search_flights`: `Search for flights by route and date. Returns cash-priced options ranked for the traveler — weighing their airline loyalty/status and trave…`
- `search_hotels`: `Search for hotels by location and dates. Returns a list of matching hotels with cash and points rates and deal scores. To produce a focused…`
- `search_vehicles`: `Search for rental vehicles at an airport or city. Returns available cars sorted by price with vendor, class, and rate details.`
- `update_traveler_profile`: `Save a learned travel preference or experience to the user's traveler profile. Use when the user shares preferences, likes, dislikes, or tr…`

## Changes

- 2026-09-26: [count changed, description changed, tool added](../../deltas/2026-09-26/9dc511da618e354e45d7.json): `1 tool(s) added; 4 field(s) changed`
- 2026-09-25: [description changed, schema changed](../../deltas/2026-09-25/9dc511da618e354e45d7.json): `7 field(s) changed`
- 2026-09-24: [count changed, tool added](../../deltas/2026-09-24/9dc511da618e354e45d7.json): `4 tool(s) added; signals: imperative_language_introduced` **(notable)**
- 2026-09-23: [schema changed](../../deltas/2026-09-23/9dc511da618e354e45d7.json): `4 field(s) changed`
- 2026-09-10: [annotation changed, description changed, schema changed](../../deltas/2026-09-10/9dc511da618e354e45d7.json): `17 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-09-09: [count changed, description changed, schema changed, tool added](../../deltas/2026-09-09/9dc511da618e354e45d7.json): `1 tool(s) added; 4 field(s) changed`
- 2026-09-05: [annotation changed, count changed, description changed, schema changed, tool added](../../deltas/2026-09-05/9dc511da618e354e45d7.json): `2 tool(s) added; 14 field(s) changed`
- 2026-09-04: [count changed, description changed, schema changed, tool added](../../deltas/2026-09-04/9dc511da618e354e45d7.json): `1 tool(s) added; 5 field(s) changed; signals: length_more_than_doubled`
- 2026-09-03: [description changed, schema changed](../../deltas/2026-09-03/9dc511da618e354e45d7.json): `9 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-09-01: [count changed, description changed, schema changed, tool added](../../deltas/2026-09-01/9dc511da618e354e45d7.json): `6 tool(s) added; 10 field(s) changed`
- 2026-08-28: [schema changed](../../deltas/2026-08-28/9dc511da618e354e45d7.json): `146 field(s) changed`
- 2026-08-27: [annotation changed, description changed, schema changed](../../deltas/2026-08-27/9dc511da618e354e45d7.json): `481 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-08-25: [count changed, tool added](../../deltas/2026-08-25/9dc511da618e354e45d7.json): `1 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.gondola.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
