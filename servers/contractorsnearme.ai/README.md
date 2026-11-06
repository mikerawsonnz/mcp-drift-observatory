# contractorsnearme.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/contractorsnearme.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://contractorsnearme.ai/api/mcp` | 14 | [`342340c7fdbd`](b25a273be4905f675e5d.json) | 2026-09-02 |

## Tools at `https://contractorsnearme.ai/api/mcp`

- `get_availability`: `Get a contractor's published availability calendar by slug. Returns days, start/end times, timezone, and note. Public read, no API key requ…`
- `get_contractor`: `Get detailed contractor profile by slug. Returns full profile including about text, contact info, and trade details.`
- `get_itb`: `Get a single public invitation to bid (ITB) by its UUID. Returns full project detail including description, budget range, job site address,…`
- `get_marketplace_request`: `Get a single public marketplace request by UUID or slug, with canonical request status, bounded budget visibility, payment summary, and pro…`
- `get_my_leads`: `Get leads submitted to the authenticated contractor's directory profile. Requires API key authentication. Returns lead name, email, phone,…`
- `get_reviews`: `Get reviews for a contractor by slug. Returns review text, rating, reviewer name, and dates. Limited to 50 per request.`
- `list_marketplace_requests`: `List public marketplace requests with canonical request status, bounded budget visibility, urgency, payment summary, and proposal/applicati…`
- `list_trades`: `Get a list of all available trades/professions. Returns filtered list of contractor trades from the directory.`
- `respond_to_lead`: `Update the status of a lead owned by the authenticated contractor's directory profile, optionally adding a note. Requires API key authentic…`
- `search_contractors`: `Search active contractors by trade, location, company name, and geo radius.`
- `search_itbs`: `Search public invitations to bid (ITBs) on the projects board. Returns open project title, description, budget range, location, and created…`
- `submit_lead`: `Submit a lead to ContractorsNearMe. Requires API key authentication.`
- `submit_review`: `Submit a review for a contractor. Requires API key authentication. Reviews are held for moderation before publishing.`
- `update_my_profile`: `Update the authenticated contractor's own directory profile. Requires API key authentication. Only the profile owned by the key's contracto…`

## Changes

- 2026-09-02: [count changed, schema changed, tool added](../../deltas/2026-09-02/b25a273be4905f675e5d.json): `2 tool(s) added; 10 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://contractorsnearme.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
