# api.cactal.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.cactal.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.cactal.ai/v1/mcp` | 84 | [`a793a25f671a`](1e88271a5dc384289225.json) | 2026-11-06 |

## Tools at `https://api.cactal.ai/v1/mcp`

- `cms_collections_create`: `Creates a collection in the website’s CMS. 'slug' uses lowercase letters, digits, and hyphens (max 64 characters, starting with a letter) a…`
- `cms_collections_delete`: `Soft-deletes the collection, making it and all of its items unreachable through the API; the slug becomes reusable. Refused with a conflict…`
- `cms_collections_update`: `Updates 'displayName' (1–200 characters), 'description' (up to 2,000 characters; pass 'null' to clear), and/or 'slug' (a rename). A slug ch…`
- `cms_fields_create`: `Adds a typed field at the end of the collection’s field order. 'key' is lowercase snake_case (max 64 characters), must be unique in the col…`
- `cms_fields_delete`: `Permanently deletes the field and its stored values: the key is stripped from every item’s 'data', and reference or asset attachments made…`
- `cms_fields_update`: `Updates 'displayName', 'description', 'required', 'isUnique', 'example', and (for 'option' fields only) 'config'; 'type' and 'targetCollect…`
- `cms_items_backreferences_list`: `Lists active items that reference the target item through a 'reference' or 'multi_reference' field, newest first, with cursor pagination (d…`
- `cms_items_create`: `Creates an item at the end of the collection’s manual order. Scalar values go in 'data' keyed by field key and are validated against the fi…`
- `cms_items_delete`: `Soft-deletes the item: it disappears from reads, list results, and backreferences, and fields referencing it read 'null' (single reference)…`
- `cms_items_get`: `Returns one item, looked up by 'itemId' or by the 'collectionId' + 'slug' pair (provide exactly one of the two). The 'data' object is compl…`
- `cms_items_list`: `Returns the collection’s active items in manual (drag) order by default, 20 per page (max 100); paginate with 'cursor' or with 1-based 'pag…`
- `cms_items_restore`: `Restores a soft-deleted item, making it readable again and re-exposing references to and from it. Returns 404 when the item is not currentl…`
- `cms_items_setPublished`: `Use exactly one publication action: 'published: true' publishes immediately and sets 'publishedAt' to now; a future 'publishAt' schedules a…`
- `cms_items_update`: `Patches an item; omitted fields are left untouched. Keys in 'data' are merged into the existing values and validated the same way as on cre…`
- `cms_schema_snapshot`: `Returns every active collection and field of a website in one call — the full content model. Collections are ordered newest first; fields a…`
- `docs_read`: `Read one Cactal documentation page as Markdown. Pass a page path from docs search results, for example "concepts/publishing" or "agents/age…`
- `docs_search`: `Search the Cactal product documentation: concepts, guides, agent workflows, platform limits, and the API reference. Returns matching Markdo…`
- `feedback_submit`: `Adds user-requested free-form feedback to the Cactal product-feedback inbox. Describe what happened and what would have made the experience…`
- `profile_get`: `Returns who this credential acts for (a stable 'id', plus 'name' and 'email' for a person) and the organizations it can work in. An organiz…`
- `skills_read`: `Read the matching Cactal skill before acting: source-editing-workflow before source edits, design-direction for design, copywriting for wor…`
- `webResearch_probe`: `Renders a public page in a browser and runs measurement presets or a custom script in it, for the exact colors, type, spacing, radii, shado…`
- `webResearch_profile`: `Reads one to ten of a business's own pages (its site, Google listing, Instagram, Facebook, Yelp, or any other profile) into one Markdown pr…`
- `webResearch_screenshot`: `Renders an external public page in a real browser and returns the image, to study a reference site or the user's existing site: its layout,…`
- `webResearch_viewImage`: `Fetches 1 to 48 public image URLs and returns the pictures; nothing is stored. Up to 4 come back full size (an SVG also returns the start o…`
- `websiteAnalytics_query_get`: `Returns aggregate engagement totals — page views, distinct visitors, visits, bounces, and total time in seconds — for a date range, optiona…`
- `websiteAnalytics_realtime_get`: `Returns a compact snapshot of traffic over Umami's trailing 30-minute realtime window: total page views, distinct visitors, tracked custom…`
- `websiteAnalytics_timeseries_get`: `Returns one traffic time series bucketed by 'unit' ('year', 'month', 'day', 'hour', or 'minute'). 'series' selects which: 'pageviews' retur…`
- `websiteAssets_delete`: `Archives the asset: it immediately stops appearing in list responses and its id returns 404 from every asset endpoint. Archival cannot be u…`
- `websiteAssets_get`: `Returns the asset with 'description', 'category', and its CDN delivery shape: for transformable images 'url' is the optimized 1920px defaul…`
- `websiteAssets_importFromUrl`: `Fetches 1-10 public http(s) URLs server-side, one at a time, and stores each as a ready asset with no upload or finalize step. Media only:…`
- `websiteAssets_list`: `Returns ready assets newest first as compact rows ('description', 'category', dimensions, 'url', 'srcSet'); fetch one asset for 'originalUr…`
- `websiteAssets_update`: `Changes 'filename', 'description', or 'category'. Pass only the fields to change; 'null' clears a field. 'category' is images only.`
- `websiteDomains_createCustomDomain`: `Claims 'hostname' for this website and registers it with the Cactal edge. Custom domains must first be enabled for the website ('websiteDom…`
- `websiteDomains_list`: `Returns every domain record attached to the website, oldest first: the automatically allocated platform subdomain plus any custom domains.…`
- `websiteDomains_removeCustomDomain`: `Deregisters the hostname from the Cactal edge and deletes the domain record. If the removed domain was primary, the oldest remaining active…`
- `websiteDomains_renamePlatformDomain`: `Moves the website to '<label>.<platform domain>', the free address every website is allocated at creation. 'label' is just the leading part…`
- `websiteDomains_setPrimaryDomain`: `Makes this domain the canonical hostname for the published website: requests reaching the platform subdomain or any other custom domain are…`
- `websiteDomains_verifyCustomDomain`: `Re-checks the ownership TXT record, edge readiness, and whether an HTTPS request to the hostname reaches this Cactal domain, then returns t…`
- `websiteFavicons_set`: `Sets the website’s current favicon to a ready PNG, SVG, or ICO image from the same website asset library. Send 'assetId: null' to clear it.…`
- `websiteForms_list`: `Returns every form with inbox and spam counts, whether the published site still references it, who it notifies, the number of inbox submiss…`
- `websiteForms_recipients_add`: `Adds an email address to one form, identified by its name from the action path. New forms notify the organization owners until changed. Org…`
- `websiteForms_recipients_remove`: `Stops emailing an address for one form. A form with no recipients emails nobody; its submissions still reach the Forms inbox.`
- `websiteForms_recipients_resend`: `Issues a fresh confirmation link to a pending, failing, or stopped address.`
- `websiteForms_submissions_delete`: `Permanently deletes one submission.`
- `websiteForms_submissions_get`: `Returns one submission with its fields in submitted order.`
- `websiteForms_submissions_list`: `Returns submissions newest first as a cursor-paginated page. Filter by 'form' name, 'status' ('inbox' by default, or 'spam'), and 'source'…`
- `websiteForms_submissions_setStatus`: `Moves a submission between the inbox and the spam folder. Restoring to 'inbox' sends the notification email if it was never sent. Spam is d…`
- `websiteFunctions_invoke`: `Runs one of the draft site's 'http' server functions with the website's secrets and returns its result, exactly as page code on the draft w…`
- `websiteFunctions_runs_get`: `Returns one run with its input, output, console output and outgoing requests. Secret values, in plain and common encoded forms, are redacte…`
- `websiteFunctions_runs_list`: `Lists a website's server function runs, newest first, for 'http' calls and form submissions alike. Secret values are redacted. Runs are kep…`
- `websiteKnowledge_agentNotes_edit`: `Applies exact-match text edits to the agent notes, in order; an empty 'oldStr' appends. Record only durable facts, decisions, rejected dire…`
- `websiteKnowledge_create`: `Keeps pasted or typed text as a context entry the agent searches and reads when relevant, using one of the website’s 25 slots. Cactal title…`
- `websiteKnowledge_list`: `Lists the website’s private durable context entries: uploaded files and pasted text, each with a 'title', a generated 'description', and an…`
- `websiteKnowledge_project_edit`: `Applies exact-match text edits to the user’s project knowledge text, in order; an empty 'oldStr' appends. Change it only when the user asks…`
- `websiteKnowledge_project_get`: `Returns the website’s durable project knowledge: the text the user maintains as 'content', plus the 'agentNotes' Cactal distills from agent…`
- `websiteKnowledge_read`: `Read a bounded line range from a project context document. Read short relevant documents directly; search large documents first. Do not rer…`
- `websiteKnowledge_search`: `Find evidence across selected project context documents. Batch independent queries; use passages directly when sufficient. Results merge ov…`
- `websiteKnowledge_update`: `Renames a context entry or replaces the text the agent reads. Replacing text does not change the downloadable original; images have no text.`
- `websiteKnowledge_view`: `Returns one private PNG, JPEG, or WebP context resource.`
- `websitePreview_capture`: `Renders one page of the site in a real browser and returns the image, so you can check layout, spacing, and responsive behaviour that sourc…`
- and 24 more in [1e88271a5dc384289225.json](1e88271a5dc384289225.json)

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.cactal.ai/v1/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
