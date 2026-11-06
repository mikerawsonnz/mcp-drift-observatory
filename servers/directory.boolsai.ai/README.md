# directory.boolsai.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/directory.boolsai.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://directory.boolsai.ai/mcp` | 19 | [`acd450e0cb9f`](37c4a5eda60f0a6a4dee.json) | 2026-08-20 |

## Tools at `https://directory.boolsai.ai/mcp`

- `brands_by_founder`: `List brands attributed to a founder (from Schema.org Organization markup). Useful for tracking serial DTC founders.`
- `brands_in_city`: `List indexed brands that publish a physical address in a given city. Sourced from Schema.org Organization JSON-LD.`
- `brands_in_market`: `List indexed brands explicitly serving a country market (via hreflang). Country is a 2-letter ISO code, lowercase.`
- `bulk_export`: `Paginated bulk export of indexed sites matching a filter. Returns up to 1000 rows per page in CSV or JSONL format with a cursor for continu…`
- `bulk_export_url`: `Returns a streaming-export URL for the same filter as bulk_export. Useful when the agency wants to pull 50K rows in one shot via curl/HTTP…`
- `compare_scans`: `Compare two historical scans of the same URL to surface stack changes. Returns added/removed/changed vendors, account IDs, and inline-scrip…`
- `compare_sites`: `Side-by-side stack comparison of 2-5 domains. Returns each site's vendors, account IDs, brand info, markets — and which signals are shared…`
- `directory_query`: `Unified query against the Boolsai Directory. One tool to rule the other lookups. Pass any combination of: signal_type+signal_value, domain,…`
- `domain_intel`: `Free DNS/WHOIS enrichment for a single domain. Returns: email host (Google Workspace / Microsoft 365 / etc. — derived from MX records), DNS…`
- `find_similar_by_stack`: `Find sites with the most-similar vendor stack to a given domain using Jaccard similarity over the full vendor set (not just archetype label…`
- `lookup_id`: `Cross-reference any tenant-unique account ID across the index. Useful for 'who else shares this GTM container / Klaviyo company / Sentry or…`
- `operator_cluster`: `Find every domain sharing a tenant-unique ID — the most powerful single signal in Boolsai. Given a Stripe pk_live key, Sentry DSN org, Klav…`
- `prospect_brief`: `ONE-CALL PROSPECT BRIEF for agency outbound — runs four sub-queries against the live indexed data: (1) full dossier of the prospect's stack…`
- `similar_sites`: `Find brands with similar stack archetypes to the given domain. Returns 'sites running similar tech' — useful for benchmarking, prospecting,…`
- `site_dossier`: `Full intel dossier for a single domain: detected vendors grouped by category, account IDs (GTM, GA4, Klaviyo company_id, Shopify shop_id, M…`
- `sites_using_vendor`: `List indexed sites detected using a specific vendor (e.g. 'klaviyo', 'yotpo', 'elevar', 'gorgias', 'rebuy'). Vendor slug is lowercase, unde…`
- `stack_archetype`: `List brands matching a stack archetype. Valid slugs: headless-shopify, classic-shopify-dtc, server-side-tagged, personalisation-heavy, pixe…`
- `subdomain_map`: `Every subdomain of a given root domain we've ever scanned. Reveals storefront topology — where the checkout actually lives, regional storef…`
- `summary`: `Global stats for the Boolsai directory: how many sites are indexed, signal types covered, top vendors, most-changed companies. Use at the s…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://directory.boolsai.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
