# entervista.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/entervista.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://entervista.ai/mcp` | 14 | [`03d97803c245`](1de7d28160f1d6483a49.json) | 2026-10-08 |

## Tools at `https://entervista.ai/mcp`

- `approve_request`: `Use only after the customer explicitly approves the total / quote / final price. Sends it to the business. When offered_slots is present, p…`
- `book_slot`: `Book a flat-rate service (e.g. drain cleaning) into a slot from get_availability. Returns a draft awaiting the customer's approval.`
- `cancel_request`: `Cancel an order, quote or booking on the customer's behalf.`
- `check_service_area`: `Deterministic yes/no: does this business come to the customer's zip? Returns reason, the zips it serves, excluded zips, and alternative bus…`
- `get_availability`: `Live bookable windows over the next days, from the business's own schedule (hours, crew, jobs, holds, blocks). Pass service_sku to get wind…`
- `get_business`: `Full agent-readable profile: verified identity and license, services with real prices (what's included / excluded), hours, service zips, de…`
- `get_request_status`: `Current status, ETA / arrival window, business response, and the next step. Poll this while waiting on a business.`
- `get_service_requirements`: `Before creating a request: the exact questions to ask the customer for this service (required_fields / optional_fields, each with type and…`
- `get_services`: `The business's services with pricing mode (fixed / starting_at / range / diagnostic_fee_then_quote / quote_required), price, what's include…`
- `place_order`: `Draft an order (food/retail). Returns line items, total, a ref and a customer_token. Nothing reaches the business until approve_request. As…`
- `place_service_request`: `One call for any trade job (repair, quote, booking). Pass service_sku (or a plain description and it matches one), intake_answers keyed by…`
- `request_quote`: `Ask a service business (plumber, etc.) for a price. Describe the problem in plain English. Many businesses answer instantly with an estimat…`
- `search_businesses`: `Find businesses in the network by what the customer needs (e.g. 'plumber', 'smoothie', 'clogged sink'), optionally filtered by category, zi…`
- `upload_photo`: `Stores an image and returns a URL to pass in photos[] of place_service_request. Some services require a photo (get_service_requirements say…`

## Changes

- 2026-10-08: [description changed](../../deltas/2026-10-08/1de7d28160f1d6483a49.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://entervista.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
