# autoblogging.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/autoblogging.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://autoblogging.ai/mcp` | 6 | [`10afd10c4f58`](ae5c02b56ed557b8ec58.json) | 2026-10-13 |

## Tools at `https://autoblogging.ai/mcp`

- `ask_question`: `Answer a plain-language question about Autoblogging.ai (pricing, plans, features, settings, integrations, comparisons) from its verified fa…`
- `get_brand_facts`: `Every verified fact about Autoblogging.ai: company, founder, plans and prices, credit costs, features with the plan each needs, publishing…`
- `get_page`: `The clean markdown text of any published page on autoblogging.ai (no navigation or scripts).`
- `get_pricing`: `Autoblogging.ai plans (monthly and annual USD prices, credits per month, connected sites, free monthly allowances), billing policies and th…`
- `list_features`: `Autoblogging.ai features with a one-line summary, the cheapest plan that includes each one, its credit cost and its page URL. Optionally on…`
- `search_site`: `Search every page on autoblogging.ai (features, guides, comparisons, tutorials, knowledge base) by keywords. Returns titles, URLs, markdown…`

## Changes

- 2026-10-13: [count changed, tool added](../../deltas/2026-10-13/ae5c02b56ed557b8ec58.json): `1 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://autoblogging.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
