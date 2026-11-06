# askline.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/askline.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://askline.ai/mcp` | 22 | [`2b96403d19fd`](11914e0af14c45cf83c3.json) | 2026-08-29 |

## Tools at `https://askline.ai/mcp`

- `ai_mentions`: `How often Google AI Overviews and ChatGPT mention a brand or domain (10 lookups). Costs 10 lookups.`
- `ai_search_volume`: `How often people ask ChatGPT-class tools about these keywords. Uses the saved Project market when location is omitted (1 lookup). Costs 1 l…`
- `ai_share_of_voice`: `Share of AI recommendations versus named competitors (10 lookups). Costs 10 lookups.`
- `backlink_overview`: `Backlink count, referring domains, rank, and spam score (2 lookups). Costs 2 lookups.`
- `chatgpt_answer`: `Live ChatGPT or Gemini answer for a prompt: the text, recommended brands, and cited URLs. Uses the saved Project market when location is om…`
- `competitor_keywords`: `Keywords competitors rank for that the target does not, plus overlap. Uses the saved Project when target or location is omitted. Costs 1 lo…`
- `domain_overview`: `Organic traffic, ranking keywords, and domain rank for a host. Uses the saved Project domain and market when those args are omitted. Costs…`
- `get_project`: `Return the saved Project (primary domain and market) for this MCP user. Free — not a lookup. Costs 0 lookups.`
- `gsc_pages`: `Search Console pages for the connected property. 0 credits. Costs 0 lookups.`
- `gsc_performance`: `Google Search Console totals: clicks, impressions, average position. 0 credits. Costs 0 lookups.`
- `gsc_queries`: `Search Console queries for the connected property. 0 credits. Costs 0 lookups.`
- `keyword_difficulty`: `Score how hard it is to rank in the top 10 for one or more keywords (0–100). Uses the saved Project market when location is omitted. Costs…`
- `keyword_research`: `Find related keywords with monthly search volume and keyword difficulty for a seed term. Uses the saved Project market when location is omi…`
- `link_gap`: `Referring domains that link to competitors but not the target (2 lookups). Costs 2 lookups.`
- `llm_citations`: `Pages and domains ChatGPT and AI Overviews quote for a topic or competitor. Pass a domain, a keyword, or both. ChatGPT mention data is US/E…`
- `pin_finding`: `Pin a finding to the account and SEO Board. 0 credits. Costs 0 lookups.`
- `ranked_keywords`: `Keywords a domain already ranks for, with position and volume. Uses the saved Project when target or location is omitted. Costs 1 lookup.`
- `referring_domains`: `Domains linking to the target, with rank (2 lookups). Costs 2 lookups.`
- `research_memory`: `Read or write project notes so research compounds across chats. 0 credits. Costs 0 lookups.`
- `serp_overview`: `Live Google organic SERP: ranking URLs, titles, and SERP features. Uses the saved Project market when location is omitted. Costs 1 lookup.`
- `set_project`: `Save this user's Project: primary domain and market (country + language, e.g. in-en or India English). Later keyword, SERP, and competitor…`
- `site_audit`: `On-page audit of one URL via instant pages. Stores the last run so a re-audit reports what changed (1 lookup). Costs 1 lookup.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://askline.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
