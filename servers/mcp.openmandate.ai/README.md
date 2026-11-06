# mcp.openmandate.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.openmandate.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.openmandate.ai/mcp` | 15 | [`e3c7cb16f9b1`](1be4f74ed266f8fdf331.json) | 2026-08-20 |

## Tools at `https://mcp.openmandate.ai/mcp`

- `openmandate_add_contact`: `Add a new contact for the user. A verification code (OTP) will be sent to the contact address. The user must verify the contact using openm…`
- `openmandate_close_mandate`: `Close (withdraw) a mandate. This is permanent — the mandate will stop matching and cannot be reopened. Only close if the user explicitly wa…`
- `openmandate_create_mandate`: `Create a new mandate on OpenMandate. Provide what the user is looking for (want) and what they bring to the table (offer). The user's verif…`
- `openmandate_delete_contact`: `Delete a contact. If the deleted contact was primary, the next verified contact is automatically promoted. This is permanent.`
- `openmandate_get_mandate`: `Get a mandate by ID. Returns the mandate's current status, any pending intake questions, and summary once active. Use this to check progres…`
- `openmandate_get_match`: `Get detailed information about a specific match, including compatibility grade, strengths, concerns, and — if both parties accepted — the c…`
- `openmandate_list_contacts`: `List the user's verified contacts. These are the contacts revealed to the other party on match confirmation. Each contact has an ID, type,…`
- `openmandate_list_mandates`: `List the user's open mandates. Returns non-closed mandates by default. Pass status to filter (e.g. status='closed' for history).`
- `openmandate_list_matches`: `List matches for the authenticated user. Returns matches with compatibility grade, strengths, and concerns. Check this periodically after a…`
- `openmandate_resend_otp`: `Resend the verification code for a pending contact. Use this if the user didn't receive the code or it expired (codes expire after 10 minut…`
- `openmandate_respond_to_match`: `Accept or decline a match. If you accept and the other party also accepts, contact info is revealed to both sides. Declining is permanent f…`
- `openmandate_submit_answers`: `Submit the user's answers to pending intake questions. The mandate must be in 'intake' status with pending questions. IMPORTANT: Before cal…`
- `openmandate_submit_outcome`: `Report how a confirmed match went. Available after both parties accepted and contact info was revealed. Outcomes: - 'succeeded': Found the…`
- `openmandate_update_contact`: `Update a contact's display label or set it as the primary contact. Setting a contact as primary will unset any other primary contact.`
- `openmandate_verify_contact`: `Verify a contact by submitting the OTP code sent to it. The user must check their email for the 8-digit code. After verification, the conta…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.openmandate.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
