# mcp.bamf.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.bamf.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.bamf.ai` | 177 | [`2dc5c6730a6b`](bcec739ff4350c4ddf27.json) | 2026-11-13 |

## Tools at `https://mcp.bamf.ai`

- `bamf.add_brand_font`: `Add a font file to a creator's brand fonts from an HTTPS url or file_base64. Before calling, ask the user to confirm exactly: "I have the r…`
- `bamf.add_knowledge_doc`: `Add a knowledge or memory document to a creator space. API documentation: https://bamf.ai/docs/mcp/overview`
- `bamf.add_likeness_photo`: `Save a photo of the creator to their likeness library from an HTTPS URL or a data URL, then label it. Always persist any creator photo you…`
- `bamf.add_media`: `Register an external media URL as a BAMF media asset. API documentation: https://bamf.ai/docs/mcp/overview`
- `bamf.add_memory`: `Add a short durable memory to the creator's knowledge base.`
- `bamf.admit_outreach_campaign_execution`: `Admit the exact queued campaign into executing state after rechecking current list, connector, fingerprint, and approval, returning canonic…`
- `bamf.advance_onboarding`: `Finish or skip one BAMF Bot setup step and save it on the same record as the web onboarding, so the person can continue on bamf.ai or here.…`
- `bamf.approve_outreach_campaign`: `Approve the exact prepared campaign fingerprint until an explicit expiry. Approval alone never queues or sends.`
- `bamf.archive_profile_package`: `Archive a saved Profile Studio package after exact approval. Archive is reversible through update_profile_package and never changes LinkedI…`
- `bamf.boost_post`: `Apply engagement boost to a post. Published posts boost immediately; scheduled posts are armed for publish time. Requires the posts:boost s…`
- `bamf.cancel_job`: `Cancel a queued or running BAMF async job.`
- `bamf.cancel_outreach_campaign`: `Cancel a prepared, approved, or queued campaign without invoking a provider.`
- `bamf.cancel_outreach_discovery`: `Request cancellation of one scoped outreach discovery session. This cancels discovery only and never mutates a provider campaign.`
- `bamf.check_linkedin_session`: `Check a client's LinkedIn login status in BAMF Connect and Multilogin. Agency staff keys only. Read-only.`
- `bamf.create_idea`: `Create a content idea for a creator space.`
- `bamf.create_interview_link`: `Create a secure hosted content-interview link for a creator. It returns ready-to-share copy for BAMF.ai, Slack, WhatsApp, or another connec…`
- `bamf.create_interview_transcript`: `Save an interview transcript as a BAMF knowledge document and optionally queue interview-specific knowledge processing.`
- `bamf.create_job`: `Create an async BAMF generation/research job. Prefer typed tools such as generate_post, run_research, generate_image, and generate_carousel…`
- `bamf.create_media_folder`: `Create a Media Library folder for a creator space after user approval.`
- `bamf.create_post_draft`: `Create a draft post for a creator space after the user approves exact content. Defaults to LinkedIn; pass platform=x for X drafts. Supports…`
- `bamf.create_post_request`: `Create a client post request: the BAMF team drafts it into the client's Notion content approval board (status "Post request") and is pinged…`
- `bamf.create_profile_package`: `Save a new versioned Profile Studio package after exact user approval. This reversible BAMF record write does not apply changes or publish…`
- `bamf.create_site_project`: `Create a client project destination for site artifacts. Requires sites:write; supply title and agent_lanes in params.`
- `bamf.create_video_project`: `Create a Video Studio project (viral_repurpose or talking_head) and return the artifact the BAMF work pane opens.`
- `bamf.create_x_post_draft`: `Create an X-native draft after exact approval. Use for single X posts, threads, image posts, long-form X drafts, and resource/DM campaign d…`
- `bamf.decide_client_approval`: `Record a client decision on an approval request: approved, changes_requested (comment required) or rejected; team members may only resubmit…`
- `bamf.delete_post`: `Delete a normal BAMF content post.`
- `bamf.design_post`: `Designing in the background: picks an approved reference, writes slot copy from the post, places the creator's real photo and official app…`
- `bamf.duplicate_profile_package`: `Duplicate a saved Profile Studio package as a draft variation after exact approval. This is reversible and never applies the variation to L…`
- `bamf.edit_carousel_slide`: `Edit ONE slide of an existing carousel post in place, the same as asking the in-app BAMF Bot to change one slide. Pass title/body/cta/conte…`
- `bamf.edit_post`: `Patch an existing draft or scheduled post after the user approves exact edits. Supports first comments and media fields.`
- `bamf.edit_post_image`: `Edit the post's CURRENT image in place (same path as the in-app chat image edit). Default keeps everything else the same; brand marks are l…`
- `bamf.ensure_proxy`: `Ensure a client's cloud-browser profile has a residential proxy (attaches one when missing, no-op when healthy). BAMF platform admin only.…`
- `bamf.estimate_boost`: `Estimate the projected first-wave reach (people, reactions, comments) for boosting a creator's post.`
- `bamf.find_competitor_ads`: `List the longest-running competitor ads (Meta, LinkedIn, TikTok) already tracked in the creator's workspace: advertiser, headline, copy, fo…`
- `bamf.find_funnel_examples`: `Find top AI-tagged example posts for a funnel stage (and optional format) to model a draft on: inspiration library (by likes), post templat…`
- `bamf.finish_draft`: `Finish a draft before it is shown for approval: review the whole draft end to end (every platform version, tweet, slide and image) for cohe…`
- `bamf.follow_creator`: `Follow a creator profile in a workspace.`
- `bamf.generate_carousel`: `STYLE CARDS FIRST: before the first visual of a request, call bamf.list_style_options and show the user the 4 options as a labelled 2x2 of…`
- `bamf.generate_carousel_pdf`: `Convert existing slide image URLs into a LinkedIn-ready carousel PDF and optionally attach it to a post.`
- `bamf.generate_ideas`: `Generate evidence-backed creator post ideas with source labels, why-now context, creator fit, and confidence. External research is adaptive…`
- `bamf.generate_image`: `STYLE CARDS FIRST: before the first visual of a request, call bamf.list_style_options and show the user the 4 options as a labelled 2x2 of…`
- `bamf.generate_post`: `Generate post concepts and a reviewable draft candidate from BAMF unified creator context. Defaults to LinkedIn; pass platform=x for X-nati…`
- `bamf.generate_post_edit`: `Generate a reviewable edit proposal, quality audit, deterministic quality comparison, and PATCH payload for a draft, scheduled post, or rou…`
- `bamf.generate_video`: `STYLE CARDS FIRST: before the first visual of a request, call bamf.list_style_options and show the user the 4 options as a labelled 2x2 of…`
- `bamf.generate_video_script`: `Read the video script brief for a project, or save the approved script, burned-in caption, and post copy back onto it.`
- `bamf.generate_x_post`: `Generate X-native single posts, threads, image posts, resource/auto-DM posts, long-form X posts, replies, quotes, or bookmark remixes from…`
- `bamf.get_agent_capabilities`: `Return the current BAMF app/Stack/API/MCP workflow capability map, safety contract, skill routing, and preferred tools. Use this before pla…`
- `bamf.get_agent_creator_context`: `Return a versioned, positive-projection creator context for the server-authorized creator space.`
- `bamf.get_agent_identity`: `Return the authenticated BAMF actor identity through the canonical server-resolved authority path.`
- `bamf.get_analytics_summary`: `Get LinkedIn Late-authoritative analytics totals for a creator space. Pass platform=x or use bamf.get_x_analytics_summary for X metrics.`
- `bamf.get_brain`: `Read your personal or company brain as Brain format v1 files. Returns the manifest plus BRAIN.md and the brain markdown files, with secrets…`
- `bamf.get_client_access`: `Read a client's LinkedIn access checklist: authenticator key in BAMF Vault, LinkedIn login on BAMF Cloud, Multilogin profile, BAMF Connect,…`
- `bamf.get_client_approval`: `Read one content approval request with its post and comments. Requires client_approvals:read.`
- `bamf.get_client_totp_code`: `Get the current 6-digit LinkedIn authenticator code for a client from their BAMF Vault key, so nobody relays PINs. Agency owner/admin only;…`
- `bamf.get_creator_analytics_report`: `Build a native, interactive LinkedIn analytics report across every creator space the signed-in BAMF account can access. Use for creator por…`
- `bamf.get_creator_context`: `Return the comprehensive creator context bundle for one creator space: knowledge docs, voice profile, AI analyses, integrations, interviews…`
- `bamf.get_design`: `Read a design's status, image, matched reference, template and layers (likeness, art, text). Poll after bamf.design_post. Read-only.`
- `bamf.get_funnel_mix`: `Get a creator's TOF/MOF/BOF funnel mix from tagged LinkedIn posts: per-stage counts and performance, per-format stats, the resolved goal ta…`
- `bamf.get_intelligence_processing_status`: `Read recent intelligence processing jobs for the authenticated creator, optionally limited to one resource.`
- and 117 more in [bcec739ff4350c4ddf27.json](bcec739ff4350c4ddf27.json)

## Changes

- 2026-11-13: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-13/bcec739ff4350c4ddf27.json): `7 tool(s) added; 19 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-11-12: [count changed, schema changed, tool added](../../deltas/2026-11-12/bcec739ff4350c4ddf27.json): `10 tool(s) added; 13 field(s) changed`
- 2026-11-07: [count changed, tool added](../../deltas/2026-11-07/bcec739ff4350c4ddf27.json): `3 tool(s) added`
- 2026-11-06: [count changed, description changed, tool added](../../deltas/2026-11-06/bcec739ff4350c4ddf27.json): `3 tool(s) added; 2 field(s) changed; signals: length_more_than_doubled`
- 2026-11-05: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-05/bcec739ff4350c4ddf27.json): `2 tool(s) added; 9 field(s) changed`
- 2026-11-04: [count changed, tool added](../../deltas/2026-11-04/bcec739ff4350c4ddf27.json): `2 tool(s) added`
- 2026-11-03: [count changed, tool added](../../deltas/2026-11-03/bcec739ff4350c4ddf27.json): `1 tool(s) added`
- 2026-11-02: [count changed, tool added](../../deltas/2026-11-02/bcec739ff4350c4ddf27.json): `1 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.bamf.ai"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
