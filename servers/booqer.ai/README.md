# booqer.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/booqer.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://booqer.ai/mcp` | 9 | [`b68c92cdd82b`](9bb78baa139078dd6da5.json) | 2026-11-17 |

## Tools at `https://booqer.ai/mcp`

- `cancel_booking`: `Use this when the user wants to cancel a booked local home-service appointment. Pass the cancel_url from request_booking. This cancels the…`
- `check_availability`: `Use this when the user wants to check availability for a local home-service appointment before booking. Lists the open 30-minute slots for…`
- `get_booking_status`: `Use this when the user wants to check the status of a local home-service appointment. status is confirmed, pending, canceled, or failed. No…`
- `get_business`: `Use this when the user wants to read one enrolled local home-service business and search_businesses or resolve_business already returned it…`
- `request_booking`: `Use this when the user wants to book a local home-service appointment and has already chosen an open time. Confirms the appointment when th…`
- `request_service`: `Use this when the user wants to open a quote form for a local home-service business rather than book a confirmed appointment time. Opens th…`
- `resolve_business`: `Use this when the user wants to resolve one enrolled local home-service business from a domain, a place, or a phone number. An ambiguous ma…`
- `search_businesses`: `Use this when the user wants to find a local home-service company in a city, for example "find me a gate company in Clermont, Florida", or…`
- `submit_service_request`: `Sends the user's quote request (name, email, optional phone, service location, preferred time) to the chosen business. Called by the quote…`

## Changes

- 2026-11-17: [description changed, schema changed](../../deltas/2026-11-17/9bb78baa139078dd6da5.json): `3 field(s) changed`
- 2026-11-15: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-15/9bb78baa139078dd6da5.json): `1 tool(s) added; 5 field(s) changed; signals: imperative_language_introduced` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://booqer.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
