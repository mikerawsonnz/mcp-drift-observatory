# agent.autoposter.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agent.autoposter.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agent.autoposter.ai/mcp` | 16 | [`91cefdb8eaf4`](b4c1ac88f1fe4ef8d46e.json) | 2026-11-07 |

## Tools at `https://agent.autoposter.ai/mcp`

- `autoposter_create_upload_link`: `Creates a short-lived link where the user can upload images from their device into the Auto Poster media library. Use this when the user wa…`
- `autoposter_delete_post`: `Deletes or cancels a draft, scheduled, or pending post by ID.`
- `autoposter_draft_post`: `Creates a draft post for human review. If API key lacks direct publish, post is saved as pending_approval and notifications are sent to wor…`
- `autoposter_get_analytics`: `Reads performance analytics. level 'posts' (default) returns per-post metrics (impressions, views, likes, comments, shares, clicks, ...) wi…`
- `autoposter_get_media_upload_url`: `Only for clients that can perform an HTTP PUT or multipart POST (not chat-only clients such as Gemini): if you cannot make that request you…`
- `autoposter_get_post`: `Retrieves a single post by ID including its state (drafts, pending_approval, queued, posted) and live link receipts.`
- `autoposter_get_post_status`: `Checks delivery status of a post and returns live platform links/receipts once published.`
- `autoposter_get_rules`: `Returns platform publishing constraints including character limits, media format requirements, and guidelines.`
- `autoposter_list_accounts`: `Lists all connected social media accounts (LinkedIn, X (Twitter), Instagram, TikTok, YouTube, Threads, Bluesky, Pinterest, Facebook, Telegr…`
- `autoposter_list_media`: `Lists media files (images and videos) stored in the workspace media library with public CDN URLs.`
- `autoposter_list_posts`: `Lists posts in the workspace. Supports filtering by state ('drafts', 'scheduled', 'queued', 'posted', 'failed', 'pending_approval'), captio…`
- `autoposter_publish_draft`: `Approves and immediately publishes an existing draft or pending post. Requires an API key with direct publish permission.`
- `autoposter_schedule_post`: `Schedules a post for a future date/time. Automatically converts local time using workspace/user timezone into UTC. Accepts mediaUrls (publi…`
- `autoposter_update_post`: `Edits an existing draft, scheduled, pending_approval or declined post in place: text, title, visibility, media, first comment / thread, or…`
- `autoposter_upload_media`: `Uploads an image or video to Auto Poster media library. Accepts a file object supplied by the client, a public image or video URL, a data U…`
- `get_profile`: `Return the profile represented by this request's authenticated credentials. The opaque id is unique within this app and remains unchanged a…`

## Changes

- 2026-11-07: [count changed, schema changed, tool added](../../deltas/2026-11-07/b4c1ac88f1fe4ef8d46e.json): `2 tool(s) added; 24 field(s) changed`
- 2026-11-05: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-11-05/b4c1ac88f1fe4ef8d46e.json): `10 field(s) changed`
- 2026-10-30: [schema changed](../../deltas/2026-10-30/b4c1ac88f1fe4ef8d46e.json): `2 field(s) changed`
- 2026-10-10: [schema changed](../../deltas/2026-10-10/b4c1ac88f1fe4ef8d46e.json): `18 field(s) changed`
- 2026-10-09: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-09/b4c1ac88f1fe4ef8d46e.json): `1 tool(s) added; 4 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agent.autoposter.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
