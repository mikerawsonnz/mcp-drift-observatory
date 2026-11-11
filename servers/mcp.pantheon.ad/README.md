# mcp.pantheon.ad: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.pantheon.ad.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.pantheon.ad/mcp` | 23 | [`58602f220b0d`](c385e5b261a52bf286e2.json) | 2026-11-11 |

## Tools at `https://mcp.pantheon.ad/mcp`

- `analyze_ad`: `Ads Intelligence: full AI analysis of one ad (emotional levers, biases, landing page coherence). Uses 1 Ads Intelligence credit. Runs in ba…`
- `create_brand_voice`: `Create and save a Brand Voice from a public URL or a text (uses 1 Brand Voice credit, ~1 minute).`
- `create_offer_brief`: `Create and save an Offer Brief from a public sales page URL or a text (uses 1 Offer Brief credit, ~1 minute).`
- `get_active_ads_copy`: `Copy (body, caption, CTA) of currently active ads of the monitored creators.`
- `get_competitor_active_ads`: `Active ads of a competitor the user has analyzed with Competitor Spy.`
- `get_creative_analysis`: `Saved AI analysis of an ad (awareness, hooks, mechanism, triggers, landing page coherence), if analyze_ad was run on it.`
- `get_job_status`: `Status and results of a background job started by an action tool.`
- `get_market_creators_data`: `Aggregated stats of the creators/competitors the user monitors.`
- `get_saved_ads`: `The user's swipe file, optionally filtered by competitor name.`
- `get_strategic_avatar`: `Avatar research of a project (from list_projects): pain matrix, core wound, desire chain, objections, triggers, language and strategic synt…`
- `get_top_performing_ads`: `Top performing (longest running) ads of the monitored creators.`
- `list_analyzed_pages`: `List Facebook pages the user analyzed (competitor, inspiration or brand_campaigns), with status and ad counts.`
- `list_brand_voices`: `List the user's Brand Voices (id, name).`
- `list_offer_briefs`: `List the user's Offer Briefs (id, name).`
- `list_projects`: `List the user's strategic projects (Avatar analyses) with their ids.`
- `run_ad_copilot`: `Adapt a library ad into 3 copy variants for the user's Avatar, Offer Brief and Brand Voice (uses 1 Ad Copilot credit). Runs in background:…`
- `run_brand_campaign_analysis`: `Scrape and analyze the user's own brand Meta campaigns page (uses 1 Brand Campaigns credit). Runs in background: poll get_job_status with t…`
- `run_competitor_spy`: `Scrape and analyze all ads of a competitor's Facebook page (uses 1 Competitor Spy credit). Runs in background: poll get_job_status with the…`
- `run_inspiration_search`: `Scrape and analyze a page outside the user's niche for inspiration (uses 1 Inspiration Search credit). Runs in background: poll get_job_sta…`
- `run_magic_tool`: `Summarize, translate or extract contacts/links from a text (Magic Tools). Summaries and extractions are in the language of the text; transl…`
- `run_persuasion_analysis`: `Persuasion analysis of an ad before launch: present and missing cognitive biases (uses 1 Persuasion Analysis credit). Runs in background: p…`
- `run_sales_psychology`: `Sales Psychology report for a project's Avatar + an Offer Brief (uses 1 Sales Psychology credit). Runs in background: poll get_job_status w…`
- `search_ads_library`: `Search the user's own Ads Library (ads collected by their searches) and this week's Top Ads by brand, niche, sector or copy. Returns ad ids…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.pantheon.ad/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
