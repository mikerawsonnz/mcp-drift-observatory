# api.adadvisor.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.adadvisor.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.adadvisor.ai/mcp` | 43 | [`52e47361c25d`](c151597f0d7058b04027.json) | 2026-10-31 |

## Tools at `https://api.adadvisor.ai/mcp`

- `change_entity_budget`: `Update the budget of a Meta campaign or ad set. Takes effect immediately. Provide exactly one of daily_budget or lifetime_budget in the acc…`
- `change_entity_status`: `Pause or resume one or more Meta campaigns, ad sets, or ads. Takes effect immediately. Live mutation — entities stop or start delivering on…`
- `check_lead_gen_readiness`: `Check whether this account can actually run lead gen — BEFORE building anything. Lead generation has four independent prerequisites, and ea…`
- `complete_upload`: `Push S3-uploaded files to Meta — internal helper for the Upload Creatives widget. Prefer calling upload_creatives, which opens the widget a…`
- `create_ad`: `Create one or more ads by attaching creatives to ad sets. NOT idempotent — each call creates new ads. Typical workflow: 1. search_ad_images…`
- `create_adset`: `Create one or more Meta ad sets. NOT idempotent — each call creates new ad sets. All ad sets are created as PAUSED. The targeting spec is a…`
- `create_campaign`: `Create one or more Meta ad campaigns. NOT idempotent — each call creates new campaigns. All campaigns are created as PAUSED. After creation…`
- `create_creative`: `Create one or more Meta ad creatives. NOT idempotent — each call creates new creatives. Pass a list of ''creatives'' to create several in a…`
- `create_lead_form`: `Create one or more Meta Lead Forms (instant forms) on a Facebook Page. NOT idempotent — each call creates new forms. Forms cannot be delete…`
- `create_lead_form_audience`: `Build a custom audience from how people interacted with a lead form. This is what turns lead gen into a funnel instead of a one-shot: the p…`
- `create_lookalike_audience`: `Create a lookalike audience from an existing custom audience seed. NOT idempotent — each call creates a new audience on Meta. Lookalike aud…`
- `create_website_audience`: `Create a website custom audience based on pixel events. NOT idempotent — each call creates a new audience on Meta. Common use cases: - Excl…`
- `duplicate_ad`: `Duplicate a Meta ad into the same or a different ad set. NOT idempotent — each call creates a new ad. The new ad inherits the original's cr…`
- `duplicate_adset`: `Duplicate a Meta ad set into the same or a different campaign. NOT idempotent — each call creates a new ad set. By default duplicates the a…`
- `duplicate_campaign`: `Duplicate a Meta campaign, creating a new copy in the same ad account. NOT idempotent — each call creates a new campaign. By default duplic…`
- `estimate_audience_size`: `Estimate the audience size for a targeting spec without creating anything. Use this to explore how big an audience would be before committi…`
- `get_lead_form`: `Inspect one Meta Lead Form in full — every question, disclaimer and screen. Use this whenever you need to know what a form actually ASKS. A…`
- `get_performance`: `Get performance metrics — how are my campaigns/ads doing? Use this to compare entities, find top or bottom performers, check spend and ROAS…`
- `get_pixel_health`: `Get pixel health for a Meta ad account — metadata, event counts, source and host breakdown. Returns the account's pixel(s) with: - Metadata…`
- `get_results_health`: `Is this account producing results the way it usually does? Use this to tell a real stop or drop in results from ordinary day-to-day noise,…`
- `get_timeseries`: `Get daily trend data — spot performance shifts day over day. Use this to see how a campaign, ad set, or ad is trending, detect when a perfo…`
- `init_upload`: `Get presigned S3 URLs for direct upload — internal helper for the Upload Creatives widget. Prefer calling upload_creatives, which opens the…`
- `list_ad_accounts`: `Discover and list all Meta ad accounts the user can access — start here. This is the entry point for every session. Call this FIRST to find…`
- `list_ads`: `List ads — show which creatives are running and their setup. Use this to see what ads exist, review creative details, or answer "what ads a…`
- `list_adsets`: `List ad sets — show targeting, budgets, and optimization config. Use this to see what ad sets exist, review targeting and setup, or answer…`
- `list_campaigns`: `List campaigns — show what campaigns exist, their config and budgets. Use this to see what campaigns are running, review setup before makin…`
- `list_creatives`: `List existing ad creatives for an account — use to find a creative_id for reuse with create_ad. Queries the tenant DB directly — fast index…`
- `list_custom_audiences`: `List custom audiences available for targeting in this ad account. Returns each audience's ID, name, subtype, approximate size, and delivery…`
- `list_lead_forms`: `List existing Meta Lead Forms (instant forms) for a Facebook Page. Lead forms are page-scoped (endpoint: /{page_id}/leadgen_forms), so the…`
- `list_media_assets`: `Browse this business's Creatives Hub — every media asset the platform holds. The Hub is the shared library across surfaces and agents: rend…`
- `list_pages`: `List Facebook Pages reachable for advertising from this ad account. Returns each page's id, name, the connecting user's Page-role tasks (e.…`
- `list_promotable_posts`: `List existing organic posts that can be promoted as ads. Use this to find a Facebook Page post or Instagram post the business already publi…`
- `preview_existing_creatives`: `Preview existing creatives that use the same image or video, with engagement metrics. Call this BEFORE creating a new creative to check if…`
- `register_media_assets`: `Push Creatives Hub assets to a Meta ad account and get their image hashes back. This is the ONLY way to make a generated or uploaded asset…`
- `search_ad_images`: `Search images in this account's ad library and open a visual picker to select one or more. Queries meta_ad_images by name (case-insensitive…`
- `search_ad_videos`: `Search videos in this account's ad library and open a visual picker to select one or more. Queries meta_ad_videos by title (case-insensitiv…`
- `search_targeting`: `Search targeting options — find interests, demographics, locations, behaviors. Use this before create_adset or update_adset_targeting to ge…`
- `set_lead_form_status`: `Archive or reactivate a Meta Lead Form. Archiving is the ONLY retirement path Meta offers — lead forms cannot be deleted, by us or by anyon…`
- `update_adset_targeting`: `Update the targeting for a Meta ad set. Takes effect immediately. Workflow: 1. search_targeting(search_type='interests', query='...') to fi…`
- `update_entity`: `Patch arbitrary fields on a Meta campaign, ad set, or ad. Idempotent. Long-tail edit tool. Use the dedicated change_entity_status / change_…`
- `upload_ad_image`: `Upload a single image to Meta — internal helper for the Upload Creatives widget. Prefer calling upload_creatives, which opens the widget an…`
- `upload_ad_video`: `Upload a video to Meta — internal helper for the Upload Creatives widget. Prefer calling upload_creatives, which opens the widget and runs…`
- `upload_creatives`: `Open the upload widget for adding images and videos to a Meta ad account. Opens an interactive widget where the user can: - Drag & drop or…`

## Changes

- 2026-10-31: [description changed](../../deltas/2026-10-31/c151597f0d7058b04027.json): `1 field(s) changed`
- 2026-10-30: [schema changed](../../deltas/2026-10-30/c151597f0d7058b04027.json): `9 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-10-08: [description changed, schema changed](../../deltas/2026-10-08/c151597f0d7058b04027.json): `9 field(s) changed; signals: length_more_than_doubled`
- 2026-10-07: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-07/c151597f0d7058b04027.json): `1 tool(s) added; 5 field(s) changed`
- 2026-10-03: [description changed, schema changed](../../deltas/2026-10-03/c151597f0d7058b04027.json): `74 field(s) changed; signals: length_more_than_doubled`
- 2026-09-19: [description changed](../../deltas/2026-09-19/c151597f0d7058b04027.json): `1 field(s) changed`
- 2026-09-16: [schema changed](../../deltas/2026-09-16/c151597f0d7058b04027.json): `2 field(s) changed; signals: length_more_than_doubled`
- 2026-09-15: [description changed, schema changed](../../deltas/2026-09-15/c151597f0d7058b04027.json): `39 field(s) changed; signals: length_more_than_doubled`
- 2026-09-06: [description changed, schema changed](../../deltas/2026-09-06/c151597f0d7058b04027.json): `2167 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.adadvisor.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
