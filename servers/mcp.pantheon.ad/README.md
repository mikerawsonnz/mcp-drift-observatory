# mcp.pantheon.ad: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.pantheon.ad.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.pantheon.ad/mcp` | 38 | [`c1d99fb401c1`](c385e5b261a52bf286e2.json) | 2026-11-22 |

## Tools at `https://mcp.pantheon.ad/mcp`

- `analyze_ad`: `Run a full AI analysis of one ad: emotional levers, cognitive biases and landing page coherence. Uses 1 Ads Intelligence credit. Runs in th…`
- `build_ideas_matrix`: `Build (or rebuild) the ideas matrix of an offer from the ads of its radar. Uses 1 ideas matrix credit and 1 ad label credit per ad not labe…`
- `create_brand_voice`: `Create and save a Brand Voice from a public web page or a text written by the user (about 1 minute). Uses 1 Brand Voice credit.`
- `create_offer_brief`: `Create and save an Offer Brief from a public sales page or a text describing the offer (about 1 minute). Uses 1 Offer Brief credit.`
- `get_active_ads_copy`: `Get the copy (body text, caption and call to action) of the ads currently running on the Facebook pages the user follows. Use it to study w…`
- `get_competitor_active_ads`: `Get up to 20 ads currently running for a competitor the user analyzed with Competitor Spy, found by page name.`
- `get_competitor_xray`: `Get the X-ray of a competitor page analyzed with the Competitor Spy: main angles, hooks that last, offer, gaps, style/structure/awareness m…`
- `get_creative_analysis`: `Read the saved AI analysis of one ad (awareness level, hooks, mechanism, emotional triggers, landing page coherence). Only available after…`
- `get_followed_creators_contents`: `Viral Content: posts of the creators the user follows, newest first (24 per page). times_author_median is how many times the post beat the…`
- `get_ideas_matrix`: `Get the ideas matrix of an offer: the angles (what an ad claims, to whom) and formats (style + structure) of the niche's ads, and the best…`
- `get_job_status`: `Check a background job started by an action tool and get its result when it is done. Call it again later while the status is running or pen…`
- `get_market_alerts`: `The user's latest market alerts: new pages in their sectors in the public Ads Library, the week's Top Ads in those sectors and new pages in…`
- `get_market_creators_data`: `Get summary statistics for the Facebook pages the user follows in Pantheon: total and active ads, audience, format mix and niche. Use it to…`
- `get_saved_ads`: `Get up to 20 ads from the pages in the user's swipe file, optionally only those of one competitor. Includes media links and whether each ad…`
- `get_strategic_avatar`: `Read the customer avatar research of a project: pain matrix, core wound, desire chain, objections, triggers, customer language and strategi…`
- `get_top_performing_ads`: `Get the longest-running ads of the Facebook pages the user follows. An ad that keeps running for months is usually profitable, so these are…`
- `get_viral_content`: `Viral Content: one post (caption, metrics) with the user's saved analysis in that language, if any, and the vocabulary of persuasion mechan…`
- `list_analyzed_pages`: `List the Facebook pages the user analyzed in one section of Pantheon (competitors, inspiration or own brand campaigns), with analysis statu…`
- `list_brand_voices`: `List the Brand Voices saved in the user's account. Use the ids with run_ad_copilot.`
- `list_followed_creators`: `Viral Content: the creators the user follows (platform, author_key, name, number of collected posts, last post date) and their follow limit.`
- `list_offer_briefs`: `List the Offer Briefs saved in the user's account. Use the ids with run_ad_copilot and run_sales_psychology.`
- `list_pantheon_inbox`: `Links the user sent to the Pantheon Whiteboard inbox and has not used yet (newest first).`
- `list_projects`: `List the user's Pantheon projects (customer avatar analyses). Call it first to get the project_id needed by get_strategic_avatar, run_sales…`
- `list_radar_offers`: `List the user's offers that have the radar on, with their niche and target countries. Use the ids with get_ideas_matrix and build_ideas_mat…`
- `run_ad_copilot`: `Rewrite an ad from the library into 3 copy variants for the user's audience, offer and brand voice. Uses 1 Ad Copilot credit. Runs in the b…`
- `run_brand_campaign_analysis`: `Collect and analyze the ads of the user's own brand Facebook page. Uses 1 Brand Campaigns credit. Runs in the background: call get_job_stat…`
- `run_competitor_spy`: `Collect and analyze every ad of a competitor's Facebook page from the Meta Ad Library. Uses 1 Competitor Spy credit. Runs in the background…`
- `run_competitor_xray`: `Run the X-ray of a competitor page analyzed with the Competitor Spy. Uses 1 X-ray credit and 1 ad label credit per ad not labeled yet. Tell…`
- `run_inspiration_search`: `Collect and analyze the ads of a Facebook page outside the user's niche, to borrow ideas from other markets. Uses 1 Inspiration Search cred…`
- `run_magic_tool`: `Summarize or translate a text, or extract its contacts and links (Magic Tools). Summaries and extractions keep the language of the text; tr…`
- `run_persuasion_analysis`: `Check a draft ad before launch: which persuasion biases it uses and which are missing, with suggestions. Uses 1 Persuasion Analysis credit.…`
- `run_sales_psychology`: `Write a sales psychology report that matches a project's customer avatar with an Offer Brief. Uses 1 Sales Psychology credit. Runs in the b…`
- `save_live_ads`: `Save ads found by search_meta_ads_live in the user's Pantheon library, only when the user asks. They are stored like the ads of a personal…`
- `save_viral_analysis`: `Viral Content: save your 'why it works' analysis of a post (from get_viral_content) for the user, in one language. It appears in the app on…`
- `search_ads_library`: `Search the Facebook and Instagram (Meta) ads already in Pantheon by brand, niche, sector or ad copy, in any market. This is the default way…`
- `search_meta_ads_live`: `Search the Meta Ad Library right now by keyword, in any market and language: the ads currently running, one per Facebook page, the longest…`
- `send_to_pantheon`: `Send a link to the user's Pantheon. Without a destination Pantheon picks it from the link: a TikTok, Instagram, YouTube or LinkedIn profile…`
- `show_ad_cards`: `Show ads to the user as cards in the chat (image or video, the whole ad copy, CTA, link to the Meta Ad Library and a link to open them in P…`

## Changes

- 2026-11-22: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-22/c385e5b261a52bf286e2.json): `1 tool(s) added; 28 field(s) changed; signals: length_more_than_doubled`
- 2026-11-21: [count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-21/c385e5b261a52bf286e2.json): `1 tool(s) added; 17 field(s) changed; signals: length_more_than_doubled`
- 2026-11-20: [count changed, field changed, schema changed, tool added](../../deltas/2026-11-20/c385e5b261a52bf286e2.json): `2 tool(s) added; 4 field(s) changed`
- 2026-11-17: [count changed, tool added](../../deltas/2026-11-17/c385e5b261a52bf286e2.json): `5 tool(s) added`
- 2026-11-16: [count changed, tool added](../../deltas/2026-11-16/c385e5b261a52bf286e2.json): `6 tool(s) added`
- 2026-11-14: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-11-14/c385e5b261a52bf286e2.json): `244 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.pantheon.ad/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
