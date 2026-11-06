# gigaverse.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/gigaverse.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://gigaverse.ai/api/mcp` | 5 | [`f96e9f333820`](6cc0fa07514b48a2c3a4.json) | 2026-08-20 |

## Tools at `https://gigaverse.ai/api/mcp`

- `check_roth_eligibility`: `Educational Roth IRA MAGI phase-out check using 2026 IRS limits. NOT tax or investment advice — always show the returned disclaimer to the…`
- `get_practicle_info`: `Get information about the Gigaverse PRActicle™ — a portable Roth IRA for gig workers, freelancers, and the self-employed (custody through a…`
- `get_signup_status`: `Check the status of a previously initiated signup by signup_id. Statuses: initiated (awaiting the human's confirmation), waitlist_joined (h…`
- `register_partner`: `Register a company (developer, platform, or retirement broker) as a Gigaverse integration partner. Returns a partner_id attribution slug im…`
- `start_signup`: `Initiate a Gigaverse retirement-account signup for your user. This does NOT open an account: it returns a signup_url that the HUMAN account…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://gigaverse.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
