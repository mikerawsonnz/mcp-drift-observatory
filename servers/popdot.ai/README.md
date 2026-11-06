# popdot.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/popdot.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://popdot.ai/api/mcp` | 5 | [`b40448894ec3`](154d49c3970ddc1bb1e3.json) | 2026-08-20 |

## Tools at `https://popdot.ai/api/mcp`

- `check_availability`: `Check whether a specific subdomain is available on a given domain. Returns true if the subdomain can be rented. Tip: the subdomain and doma…`
- `get_price_quote`: `Get a price quote for renting a specific domain for a given duration. Returns the computed rental cost, tier info, and pricing breakdown.`
- `rent_domain`: `Rent a subdomain, paying per-transaction with USDC on Base (x402). No funded account or stored balance: each rental is a single on-chain pa…`
- `search_domains`: `Search domains available for rent on Popdot AI. Use this when an agent needs a web address: a verifiable web identity, a temporary deployme…`
- `try_domain`: `Get a trial API key. Entry point for new agents: no payment, no human signup. Leads to a free 24-hour trial subdomain after a short screeni…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://popdot.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
