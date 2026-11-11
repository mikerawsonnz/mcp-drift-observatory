# api.athenahq.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.athenahq.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.athenahq.ai/api/mcp` | 132 | [`92166e7a5113`](d1c9dc97b241abc09e4e.json) | 2026-11-11 |

## Tools at `https://api.athenahq.ai/api/mcp`

- `add_brand_facts`: `Add brand facts to a website's Knowledge Base in bulk (1-50 per call). Each fact runs the full ingestion pipeline (deduplication, approval…`
- `add_competitors`: `Start tracking competitors on a website, 1 to 25 per call, under the same rules as the Competitors page. Each competitor needs a name and i…`
- `add_content`: `Add an article that is already written (for example, one drafted in this conversation) to the website's Content Hub as an editable draft. S…`
- `approve_brief`: `Approve a content brief and start writing the article from it. Only valid while the piece is at status generated_brief. The article is gene…`
- `check_public_ai_access`: `Check HTTP responses to AI crawler user agents and robots.txt permissions for a public website. No AthenaHQ account required. Search, retri…`
- `create_brand_kit`: `Create a brand kit from text the user provides: a name, guidance text per field (voice is the writing direction), voice settings and writin…`
- `create_content`: `Generate an article or content brief in AthenaHQ. Fetches source URLs, sends source material to external AI providers, and consumes content…`
- `create_location`: `Create a location for a website`
- `create_pillar`: `Create a Knowledge Base pillar (a subject area that groups brand facts) from a name and optional description. Get-or-create semantics: if a…`
- `create_prompt_tag`: `Create a prompt tag on a website, or return the existing tag when its name matches case-insensitively. Trims surrounding whitespace and rej…`
- `create_prompts`: `Create one or more prompts on a website`
- `create_saved_view`: `Create a saved view (filter preset) for a website. Saved views appear in the dashboard filter bar for every member of the website. filters…`
- `create_topic`: `Create a topic on a website (returns the existing topic when the name is already taken)`
- `delete_brand_facts`: `Permanently delete 1-50 brand facts from a website's Knowledge Base. There is no undo. Ids that do not exist on the website are reported in…`
- `delete_content`: `Delete a content row. Destructive: physical row delete, no undo. Powers delete-and-retry. Bulk delete is out of scope.`
- `delete_location`: `Delete a location from a website`
- `delete_pillars`: `Permanently delete 1-20 Knowledge Base pillars and every fact filed under them. Facts are deleted, not unfiled; there is no undo. Ids that…`
- `delete_prompt`: `Delete a prompt (soft when responses exist, hard otherwise)`
- `delete_topic`: `Delete a topic (soft delete; optionally also delete its prompts)`
- `draft_outreach_message`: `Draft a pitch email to the author of a cited page and save it as the page's Outreach draft, replacing any previous draft. Uses the website'…`
- `edit_content`: `Apply exact find-and-replace edits to a content draft's article body. Deterministic, no AI model involved: your replacement text lands verb…`
- `find_more_prompt_discovery`: `Find more prompts for a finished Discover run: start the next round of its series with the same sources, effort level, country, language an…`
- `find_outreach_author`: `Find who wrote a cited page and how to reach them, then save it to the page's Outreach contact. Reads the page's byline, the addresses the…`
- `get_ai_insight`: `Read one stored AI insight in full, by its id from get_ai_insights: its title, headline, body, suggested action, why it happened (with reas…`
- `get_ai_insights`: `List the website's stored AI insights: the precomputed cards on the AI Insights page, each a verified finding of one past analysis, newest…`
- `get_ai_search_value`: `AI Search Value for a website: topic-market value, captured value range, headroom, coverage, value-weighted AI share of voice, per-topic de…`
- `get_attribute_metrics`: `Get cumulative brand trait (attribute) metrics: for each brand-perception keyword (e.g. 'Affordable', 'Slow Support'), how many AI response…`
- `get_attribute_observations`: `Get individual brand trait (attribute) observations: each row is one AI response describing one entity (the brand or a competitor) with one…`
- `get_attribute_time_series`: `Get the daily trend for ONE brand trait (attribute), brand and competitors side by side — how mentions of a keyword like 'Affordable' moved…`
- `get_attributes`: `List the brand traits (called attributes in the API) tracked for a website: brand-perception keywords such as 'Affordable' or 'Slow Support…`
- `get_brand_facts`: `List a website's brand facts from the Knowledge Base, newest first, with offset paging. By default excludes facts generated by Oracle analy…`
- `get_brand_kit`: `Read a brand kit as the Brand Profile editor shows it, to inspect or change it: the draft name, the eight guidance fields as text (voice is…`
- `get_citation_rate_cumulative`: `Get cumulative citation rate — average citation rate for each competitor across the date range. citation_rate is absolute (share of all res…`
- `get_citation_rate_time_series`: `Get citation rate over time — how often AI models cite (link to) the website, grouped by day. citation_rate is absolute (share of that day'…`
- `get_competitor_attribute_metrics`: `Get brand trait (attribute) metrics per tracked competitor: for each competitor and each brand-perception keyword (e.g. 'Affordable'), how…`
- `get_competitors`: `List competitors tracked for a website`
- `get_content_citation_prompts`: `For a single tracked content item, list every prompt whose AI responses cited it — with citations, citation %, and estimated impressions. U…`
- `get_content_detail`: `Fetch the full detail of a single tracked content item — its brief and body text (drafts, optimize rewrites, snipes, authored and scraped p…`
- `get_content_draft`: `Read the current draft text of a content item — the article body as it stands right now, including every revision applied so far. Use this…`
- `get_content_hub_sheets`: `List the Content Hub tabs/sheets configured for a website. Use to discover available tabs (e.g. 1st-party content, 3rd-party placements, Re…`
- `get_content_status`: `Get the normalized pipeline status (running / succeeded / failed) for one content row, plus the raw stage behind it. Read-only. Poll once p…`
- `get_content_version`: `Read the full text of one saved version of a content item. Use it to compare two passes (fetch both and diff them yourself) or to check wha…`
- `get_content_versions`: `List the saved versions of a content item, newest first. Each entry carries its version number, label, how it was produced, and who made it…`
- `get_credit_usage`: `Read recorded organization credit consumption: total, hourly (24h) or daily trend, and charged website/group/organization pools. Use for sp…`
- `get_credit_usage_events`: `Read a page of recorded credit charges/refunds and action labels for the organization, optionally filtered by originatingWebsiteId. Use to…`
- `get_credits_organization`: `Get credit balance for the organization`
- `get_credits_website`: `Get credit balance for a specific website`
- `get_date_range`: `Get the earliest and latest response dates for a website`
- `get_group_detail`: `Fetch a single group by id with its member websites.`
- `get_group_saved_views`: `List group-level saved views (filter presets) shared across the websites in a group`
- `get_groups`: `List all groups in the organization (global API key only)`
- `get_identifiers`: `Read the identifiers of the website's brand, or of one competitor: the names, aliases and domains Athena looks for in AI responses to count…`
- `get_locations`: `List geo-locations configured for a website`
- `get_mention_rate_cumulative`: `Get cumulative mention rate — average mention rate for each competitor across the date range. mention_rate is absolute (share of all respon…`
- `get_mention_rate_time_series`: `Get mention rate over time — how often AI models mention the website by name, grouped by day. mention_rate is absolute (share of that day's…`
- `get_oracle_finding`: `When grounding is present, use its complete team-confirmed statement and all supporting facts as joint evidence; the legacy fact ID/text ar…`
- `get_oracle_findings`: `When grounding is present, use its complete team-confirmed statement and all supporting facts as joint evidence; the legacy fact ID/text ar…`
- `get_personas`: `List personas configured for a website with per-persona prompt counts. Use it to resolve persona_id values returned by other tools to perso…`
- `get_pillar_document`: `Fetch a pillar's synthesized markdown document from the Knowledge Base. Returns document: null when the pillar exists but has no synthesize…`
- `get_pillars`: `List a website's Knowledge Base pillars (excluding archived ones) with approved-fact counts, whether a synthesized document exists, and whe…`
- and 72 more in [d1c9dc97b241abc09e4e.json](d1c9dc97b241abc09e4e.json)

## Changes

- 2026-11-11: [count changed, tool added](../../deltas/2026-11-11/d1c9dc97b241abc09e4e.json): `4 tool(s) added`
- 2026-11-10: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-10/d1c9dc97b241abc09e4e.json): `2 tool(s) added; 8 field(s) changed; signals: length_more_than_doubled`
- 2026-11-07: [count changed, tool added](../../deltas/2026-11-07/d1c9dc97b241abc09e4e.json): `2 tool(s) added`
- 2026-11-06: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-06/d1c9dc97b241abc09e4e.json): `11 tool(s) added; 26 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-11-04: [schema changed](../../deltas/2026-11-04/d1c9dc97b241abc09e4e.json): `1 field(s) changed`
- 2026-11-02: [schema changed](../../deltas/2026-11-02/d1c9dc97b241abc09e4e.json): `3 field(s) changed`
- 2026-10-29: [count changed, tool added](../../deltas/2026-10-29/d1c9dc97b241abc09e4e.json): `2 tool(s) added`
- 2026-10-28: [count changed, tool added](../../deltas/2026-10-28/d1c9dc97b241abc09e4e.json): `1 tool(s) added`
- 2026-10-25: [schema changed](../../deltas/2026-10-25/d1c9dc97b241abc09e4e.json): `1206 field(s) changed`
- 2026-10-24: [description changed, schema changed](../../deltas/2026-10-24/d1c9dc97b241abc09e4e.json): `4 field(s) changed; signals: length_more_than_doubled`
- 2026-10-23: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-23/d1c9dc97b241abc09e4e.json): `1 tool(s) added; 14 field(s) changed`
- 2026-10-22: [count changed, tool added, tool removed](../../deltas/2026-10-22/d1c9dc97b241abc09e4e.json): `10 tool(s) added; 4 tool(s) removed`
- 2026-10-20: [annotation changed, description changed, schema changed](../../deltas/2026-10-20/d1c9dc97b241abc09e4e.json): `3 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.athenahq.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
