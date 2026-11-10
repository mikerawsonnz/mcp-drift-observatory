# api.bluerate.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.bluerate.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.bluerate.ai/mcp` | 3 | [`86968d8c3a94`](8480c0b3b383f5f74749.json) | 2026-11-10 |

## Tools at `https://api.bluerate.ai/mcp`

- `get_loan_officer`: `Get one loan officer's bluerate.ai profile by NMLS ID: name, company, licensed states, loan types, languages, about text, up to 3 client re…`
- `request_callback`: `Ask a loan officer listed on bluerate.ai to call the user back. Returns confirmationUrl, a one-time bluerate link valid for 24 hours: give…`
- `search_loan_officers`: `Find licensed US mortgage loan officers listed on bluerate.ai by state, optionally near a city or ZIP code, for a loan type (conventional,…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.bluerate.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
