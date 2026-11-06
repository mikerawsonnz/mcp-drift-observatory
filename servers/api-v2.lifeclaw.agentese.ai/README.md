# api-v2.lifeclaw.agentese.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api-v2.lifeclaw.agentese.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api-v2.lifeclaw.agentese.ai/mcp` | 16 | [`c32ffb1440b3`](a36f138754e21f19be81.json) | 2026-10-14 |

## Tools at `https://api-v2.lifeclaw.agentese.ai/mcp`

- `account_status`: `Points balance, display name, and the selected receiving number for call_me (masked). Use receiving_phone_status for setup and caller_id_st…`
- `call_business`: `Phone a business and wait for the outcome. 'action="book"': reserve. Required: merchant_name, date (YYYY-MM-DD), time_ (HH:MM, 24h), party_…`
- `call_contact`: `Call a saved private contact without passing their full number. First list_contacts and confirm the chosen name, masked number and exact sp…`
- `call_me`: `Ring the user's own phone, read them 'message', and bring back what they say. A phone call interrupts the user. Follow their explicit instr…`
- `call_person`: `Call one private person and relay one message from the user. Ask the user to confirm the recipient, E.164 number and exact spoken message f…`
- `caller_id_status`: `Check the owner's outbound Caller ID. Verified plus enabled display enables call_person. call_me uses a separate receiving number. If setup…`
- `delete_contact`: `Delete a saved contact by exact name after the user confirms deletion.`
- `get_place`: `Full details for one place from search_places: phone, hours, rating, website, booking link. Pass the same 'location' you searched with. 'ph…`
- `list_bookings`: `The account's bookings (confirmed, cancelled, answered inquiries). 'status' filters: "confirmed", "cancelled", "answered", or "" for all.`
- `list_contacts`: `List the token owner's saved contacts with masked phone numbers. Each contact_ref pins the current name and number for call_contact. If two…`
- `modify_booking`: `Phone the venue to cancel or reschedule a confirmed booking from list_bookings. 'action' is "cancel" or "reschedule"; reschedule needs new_…`
- `receiving_phone_status`: `Check where call_me would ring (masked). A number must be explicitly selected and verified by voice; SMS login alone does not qualify. The…`
- `save_contact`: `Add or update one contact after confirming name and number with the user. phone_number must be E.164, e.g. +85291234567. This updates the s…`
- `search_places`: `Search businesses (restaurants, salons, clinics, hotels…) by free text. 'location' is REQUIRED and decides which country is searched — a ci…`
- `update_contact`: `Edit a saved contact's name and/or E.164 phone number atomically. Confirm the existing contact and proposed change with the user first. A n…`
- `wait_for_call`: `Keep waiting for a call that call_business / modify_booking / call_person / call_me reported as in_progress. Returns the flat result once t…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api-v2.lifeclaw.agentese.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
