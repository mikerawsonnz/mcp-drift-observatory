# agentsindex.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agentsindex.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agentsindex.ai/mcp` | 12 | [`e0c85b841395`](ae90c62287403cba0474.json) | 2026-11-09 |

## Tools at `https://agentsindex.ai/mcp`

- `compare_listings`: `Two tools side by side, as markdown: taglines, pricing, API availability, tags — the researched compare facts, honest about unknowns.`
- `create_order`: `Turns a quote (from get_quote) into an order, payable for 24 hours. Same account as the quote: its session Cookie header, or its agent key…`
- `get_best_of`: `The Published tools in one category, in the order its category page prints (ranked by what we can confirm: a public price, an API and docs,…`
- `get_listing`: `One tool in full, as answer-first markdown: the summary, then every question on the sheet with its answer, the vendor's own words for it an…`
- `get_quote`: `A signed price for one offer (from list_offers) on one listing, valid for a short time, and whether the listing can have it now. Only the a…`
- `list_categories`: `AgentsIndex's categories with their live listing counts, 0 for one with none yet.`
- `list_offers`: `What a listing owner can buy on AgentsIndex, with prices in US cents excl. VAT, each offer's term and what it needs. Keyless. Same answer a…`
- `my_listings`: `What the AgentsIndex owner dashboard shows about the listings an account owns: each one's status ('status.kind': review with the expected d…`
- `search_listings`: `Full-text search over AgentsIndex's Published tools. Returns compact records (name, slug, tagline, url). Fetch depth with get_listing.`
- `send_lead`: `Send a buyer-intent enquiry (lead) to a tool or a whole category on AgentsIndex. Keyless. Requires consent:true, a real name, a permanent (…`
- `submit_listing`: `Submit a tool to AgentsIndex: the url alone; we write its name and description from its own pages. Requires an existing signed-in account w…`
- `subscribe_newsletter`: `Subscribe an email to the AgentsIndex digest of new and freshly re-verified tools. Provide an email; returns { ok }. The address gets one m…`

## Changes

- 2026-11-09: [description changed](../../deltas/2026-11-09/ae90c62287403cba0474.json): `1 field(s) changed`
- 2026-11-06: [description changed](../../deltas/2026-11-06/ae90c62287403cba0474.json): `1 field(s) changed`
- 2026-11-03: [description changed](../../deltas/2026-11-03/ae90c62287403cba0474.json): `1 field(s) changed`
- 2026-11-01: [description changed](../../deltas/2026-11-01/ae90c62287403cba0474.json): `1 field(s) changed`
- 2026-10-31: [description changed](../../deltas/2026-10-31/ae90c62287403cba0474.json): `1 field(s) changed`
- 2026-10-27: [description changed](../../deltas/2026-10-27/ae90c62287403cba0474.json): `1 field(s) changed`
- 2026-10-26: [description changed](../../deltas/2026-10-26/ae90c62287403cba0474.json): `2 field(s) changed`
- 2026-10-25: [description changed](../../deltas/2026-10-25/ae90c62287403cba0474.json): `1 field(s) changed`
- 2026-10-24: [description changed](../../deltas/2026-10-24/ae90c62287403cba0474.json): `2 field(s) changed`
- 2026-10-21: [description changed](../../deltas/2026-10-21/ae90c62287403cba0474.json): `2 field(s) changed`
- 2026-10-20: [description changed](../../deltas/2026-10-20/ae90c62287403cba0474.json): `1 field(s) changed; signals: url_introduced`
- 2026-10-19: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-19/ae90c62287403cba0474.json): `4 tool(s) added; 7 field(s) changed; signals: length_more_than_doubled, url_introduced`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agentsindex.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
