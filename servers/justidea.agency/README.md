# justidea.agency: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/justidea.agency.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://justidea.agency/mcp` | 8 | [`c28676f3d501`](20b549032a4f19d5b70d.json) | 2026-10-13 |

## Tools at `https://justidea.agency/mcp`

- `get_page`: `Full text of one justidea.agency page as Markdown: a service, a price list, the company profile, reviews, a blog article. Accepts a full UR…`
- `get_scan_result`: `Result of a scan started with scan_analytics, scan_ai_visibility or scan_google_visibility that was still running. Returns the same grade a…`
- `list_services`: `List JustIdea Agency services with the published starting ("from") prices and links. Returns the price list (12 service categories, each wi…`
- `scan_ai_visibility`: `Free check of how ready a website is for AI assistants and AI search (ChatGPT, Perplexity, Gemini, Claude): whether their crawlers get in (…`
- `scan_analytics`: `Free check of how a website or online store measures traffic and sales: Google Tag Manager, GA4 and e-commerce events, consent banner and C…`
- `scan_google_visibility`: `Free check of whether Google can index a website well: Googlebot access in robots.txt and on the server, noindex, canonical, http-to-https…`
- `search_site`: `Search justidea.agency pages by titles, descriptions and section headings. Polish and English queries both work. Returns titles, URLs and d…`
- `send_inquiry`: `Send a sales inquiry to JustIdea Agency (Kraków, Poland) on behalf of the user. It goes to the agency CRM and the sales team, the sender ge…`

## Changes

- 2026-10-13: [schema changed](../../deltas/2026-10-13/20b549032a4f19d5b70d.json): `10 field(s) changed`
- 2026-10-10: [count changed, description changed, tool added](../../deltas/2026-10-10/20b549032a4f19d5b70d.json): `1 tool(s) added; 1 field(s) changed; signals: url_introduced`
- 2026-10-04: [count changed, tool added](../../deltas/2026-10-04/20b549032a4f19d5b70d.json): `3 tool(s) added; signals: url_introduced`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://justidea.agency/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
