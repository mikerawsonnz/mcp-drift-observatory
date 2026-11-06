# 4ai.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/4ai.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://4ai.ai/mcp` | 10 | [`17272ff57c90`](d22db45d94128c733636.json) | 2026-11-02 |

## Tools at `https://4ai.ai/mcp`

- `ai_domain_sales`: `The biggest publicly reported .ai domain sales (price in USD, date, venue, source). Useful to estimate what a .ai domain is worth.`
- `compare_domains`: `Compare 2 to 5 .ai domain names side by side: length, type, words, whether 4ai sells it, estimated value ranges and a short verdict.`
- `estimate_domain_value`: `Free value estimate for any .ai domain name: auction, marketplace and brokerage values with likely ranges, the type of name, a short verdic…`
- `get_domain`: `Details for one domain in the 4ai portfolio (for example "p0.ai"): categories, page, offer link, and comparable public .ai sales. Says so i…`
- `get_offer_link`: `A link to the offer form for a 4ai domain with the amount (and an optional note) filled in. Nothing is sent: the user opens the link, check…`
- `how_buying_works`: `The steps, payment (Escrow.com), fees, minimum offer and transfer time for buying a .ai domain from 4ai. Use it when the user asks whether…`
- `list_categories`: `Categories of .ai domains in the 4ai portfolio, with what they are good for and how many names each has.`
- `search_domains`: `Search the 4ai.ai portfolio of premium .ai domain names for sale. Filter by a word in the name, a category (see list_categories), type and…`
- `similar_domains`: `Alternatives to a .ai domain: give any name (taken, too expensive, or one the user already likes) and get the closest .ai domains that are…`
- `suggest_domains`: `Describe a company, product or idea in plain words (e.g. "telehealth app for mental health", "crypto casino", "quantum chip startup") and g…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://4ai.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
