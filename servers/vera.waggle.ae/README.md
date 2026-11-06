# vera.waggle.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/vera.waggle.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://vera.waggle.ae/v1/mcp` | 16 | [`f808897dd300`](d06c15457e98ec8c8b45.json) | 2026-10-24 |

## Tools at `https://vera.waggle.ae/v1/mcp`

- `ai_answers`: `Put a buyer's question to an AI assistant that searches the live web, and see whether a brand and its competitors are named in the answer,…`
- `company_profile`: `Given a company's domain, read its homepage and up to 3 standard pages (about, contact, team) and return a profile: name, description, logo…`
- `company_serp_footprint`: `Audit a company's SERP digital footprint, brand reputation, owned domains, and entity profiles. Separates owned web properties, social/enti…`
- `extract_contacts`: `Read one public page and return the contact details it publishes: email addresses, phone numbers, social profile links and links to contact…`
- `extract_local_places`: `Extract Google Local Pack (3-pack) and Google Places listings for local queries. Returns place_id/cid, title, rating, review count, address…`
- `extract_products`: `Read one public product page and return the product data it publishes in its structured markup: name, brand, SKU or GTIN, and offers with p…`
- `extract_shopping_results`: `Extract Google Shopping carousel listings for e-commerce and product queries. Returns product title, price, currency, merchant, rating, rev…`
- `find_discussion_candidates`: `Search Google and filter organic results (positions 1-100) specifically for community discussions and forum threads (Reddit, Quora, HackerN…`
- `geo_citation_radar`: `Run GEO Citation & Injection Radar for a topic query and brand. Calculates citation probability score (0-100), identifies high-impact Reddi…`
- `google_serp`: `Execute a full Google SERP search query with strict Google provenance (depth 10 to 100). Returns verified Google organic results with class…`
- `keyword_ideas`: `Keyword ideas for a seed keyword from Google autocomplete (the seed plus question words or the alphabet), People Also Ask and related searc…`
- `scrape`: `Read one public web page and return its content: the main text (as Markdown with response_format="markdown"), links, metadata and a quality…`
- `search`: `Search Google and return the results: titles, URLs and snippets, plus Google's own answer boxes, People Also Ask and related searches when…`
- `seo_audit`: `Audit one public page's technical SEO and how ready it is for AI search: title, description, canonical, robots and indexing directives, hea…`
- `sitemap`: `Read a site's sitemap.xml (or a sitemap index) and return the page addresses it lists, up to limit (100 by default), optionally only those…`
- `youtube_transcript`: `Return the transcript of one public YouTube video as text. Costs 6 credits per started minute of video (a 10-minute video costs 60), up to…`

## Changes

- 2026-10-24: [description changed, schema changed](../../deltas/2026-10-24/d06c15457e98ec8c8b45.json): `5 field(s) changed`
- 2026-10-22: [count changed, description changed, tool added](../../deltas/2026-10-22/d06c15457e98ec8c8b45.json): `8 tool(s) added; 1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://vera.waggle.ae/v1/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
