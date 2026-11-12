# api.bluerate.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.bluerate.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.bluerate.ai/mcp` | 3 | [`a57c465b405d`](8480c0b3b383f5f74749.json) | 2026-11-12 |

## Tools at `https://api.bluerate.ai/mcp`

- `get_loan_officer`: `Returns one loan officer's bluerate.ai profile by NMLS ID: name, company, licensed states, loan types, languages, about text, up to 3 clien…`
- `request_callback`: `Creates a one-time bluerate.ai link (confirmationUrl, valid for 24 hours) for asking a loan officer listed on bluerate.ai to call back. The…`
- `search_loan_officers`: `Searches licensed US mortgage loan officers listed on bluerate.ai by state, optionally near a city or ZIP code, for a loan type (convention…`

## Changes

- 2026-11-12: [annotation changed, description changed, schema changed](../../deltas/2026-11-12/8480c0b3b383f5f74749.json): `4 field(s) changed`
- 2026-11-11: [description changed, schema changed](../../deltas/2026-11-11/8480c0b3b383f5f74749.json): `5 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.bluerate.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
