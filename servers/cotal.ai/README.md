# cotal.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/cotal.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://cotal.ai/mcp` | 12 | [`bb33a1698bf9`](07baf0981b282254a93a.json) | 2026-10-15 |

## Tools at `https://cotal.ai/mcp`

- `cotal_draft_post`: `Stages a new article for the COTAL build log (cotal.ai/blog). It lands as a draft unless you submit it for review (status pending), and goe…`
- `cotal_get_my_post`: `One staged article with every field, its current markdown and its revision history; pass revision for an older text. Requires a team key.`
- `cotal_get_post`: `Returns one build-log post as markdown (title, summary, date, author, full body) by its slug. Get slugs from cotal_list_posts or cotal_sear…`
- `cotal_join_waitlist`: `Reserves a seat on the waitlist for Cotal Cloud, the hosted Cotal mesh (closed alpha), for the user's email. Idempotent per email: calling…`
- `cotal_list_my_posts`: `The review state of the articles staged on this site : slug, title, status (draft, pending, published, rejected), review note and current r…`
- `cotal_list_posts`: `Lists posts from the COTAL build log (blog), newest first, with cursor pagination. Each item has slug, title, summary, date, author and URL…`
- `cotal_overview`: `Returns a structured overview of COTAL: what it is, who it is for, when to use it, how to install it, the site's API and MCP surface, prici…`
- `cotal_request_call`: `Sends a discovery-call request to the COTAL founders for a company evaluating agent coordination. The team replies by email. Requires the u…`
- `cotal_search`: `Keyword search over the COTAL build log (blog posts) and the key documentation and site pages. Returns ranked results with canonical and ma…`
- `cotal_submit_feedback`: `Files feedback (bug, idea, friction, praise, other) with the COTAL team on behalf of the user. The same log the site's feedback widget writ…`
- `cotal_subscribe_newsletter`: `Subscribes the user's email to release updates from the COTAL team. Idempotent: an already-subscribed email is a no-op.`
- `cotal_update_post`: `Improves an article staged with cotal_draft_post. A changed title, dek or body becomes a new revision; sending the text it already has chan…`

## Changes

- 2026-10-15: [count changed, tool added](../../deltas/2026-10-15/07baf0981b282254a93a.json): `4 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://cotal.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
