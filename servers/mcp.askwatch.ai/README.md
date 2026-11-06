# mcp.askwatch.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.askwatch.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.askwatch.ai/gsc` | 11 | [`39be7cf70098`](3daa083ca9742034313f.json) | 2026-09-26 |

## Tools at `https://mcp.askwatch.ai/gsc`

- `brand_split`: `Branded versus non-branded search, split on the words supplied. The split is only as good as those terms: misspellings and the domain name…`
- `changes`: `What gained and what lost between this period and the one before it, with small rows filtered out. Answers 'what dropped in the last 28 day…`
- `find_cannibalization`: `Queries where more than one page of the site is being shown, with how each page does on them.`
- `find_opportunities`: `Queries ranking 5-20 with plenty of impressions but a click-through rate below what is typical at their position — where a title or snippet…`
- `inspect_url`: `Google's index status for one URL, as the URL Inspection API reports it: whether it is indexed, when it was last crawled, and which canonic…`
- `list_sitemaps`: `Sitemaps submitted for the property and their status, from Google's Sitemaps API. Read-only: submitting is not possible with read access.`
- `list_sites`: `Search Console properties this connection can read, from Google's Sites API. These are the exact strings the site argument takes.`
- `page_queries`: `What searches a specific page is shown for.`
- `query`: `Direct query against Google's Search Analytics API, with the same dates, dimensions and filters it takes, passed through unchanged.`
- `site_overview`: `How the site did over a period compared with the one before it: clicks, impressions, CTR, average position and the change in each. Covers t…`
- `top`: `Top queries, pages, countries or devices for a period. Optionally narrowed to one country or device — 'top pages in Germany on mobile' is o…`

## Changes

- 2026-09-26: [field changed](../../deltas/2026-09-26/3daa083ca9742034313f.json): `22 field(s) changed`
- 2026-09-24: [annotation changed, description changed, field changed](../../deltas/2026-09-24/3daa083ca9742034313f.json): `61 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.askwatch.ai/gsc"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
