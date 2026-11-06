# mcp.dotsy.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.dotsy.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.dotsy.ai/mcp` | 91 | [`8a733239923e`](d4adb947e2c6cbd354fa.json) | 2026-10-13 |

## Tools at `https://mcp.dotsy.ai/mcp`

- `adapt_site_analyze`: `Propose nav wiring + blog collectionization for an imported mirror (draft, opt-in). Read-only; returns per-adapter reports + proposalEtag.…`
- `adapt_site_apply`: `Apply the adapt proposal (draft): wire nav into the menu store and/or rewrite the blog index to a live <dotsy-collection>. One undo covers…`
- `adapt_site_revert`: `Atomically restore everything the last adapt_site_apply wrote (fragments, the menu doc when the op touched it, index, member configs, route…`
- `add_custom_domain`: `Connect apex and/or www on a paid plan; starts a DNS connect session.`
- `apply_changeset`: `Atomic writes[] + deletes[]; attach routes via writes[].route. At most 10 writes; each body ≤60KB and the call ≤80KB. Larger new pages: sta…`
- `batch_patch_content`: `patch_content on multiple keys; all-or-nothing validation. Preferred edit path for pages over 60KB. replace-string value/replace ≤60KB; who…`
- `bulk_put_assets`: `Upload 1–200 CMS assets; key = path after /assets/. Each item: exactly one of bodyBase64, bodyText (plain text for .css/.js/.mjs/.json/.svg…`
- `bulk_put_content`: `Stage many content keys (pages, layouts, fragments). Content only — not routes or assets. Each body ≤60KB and the whole call ≤80KB; larger…`
- `claim_site`: `Move the guest draft onto your signed-in Dotsy account. Requires OAuth Connect; pass the guestToken from start_site.`
- `create_site`: `Create empty site; seeds brief. Globally taken slugs auto-suffix to '{slug}-{adjective}-{noun}' (default); pass onSlugTaken:"fail" to get a…`
- `decompose_analyze`: `Deprecated — use structure_site_analyze.`
- `delete_asset`: `Delete a static asset by key. The editor and draft preview drop it at once; the published site drops it at the next publish.`
- `delete_content`: `Delete content key (tombstone if published). A fragments/* section that pages still place is refused with section_in_use (lists the pages)…`
- `delete_draft_test`: `Remove a draft A/B test (releases variant bodies; does not publish).`
- `delete_menu_item`: `Remove one item from a menu (page stays live).`
- `delete_route`: `Remove a route by path.`
- `delete_site`: `Permanently delete site; confirmSlug must equal slug.`
- `detach_section`: `Give one page its own copy of a shared section; every other page keeps the shared one. A draft — publish_site to go live. A section the lay…`
- `discard_drafts`: `Discard unpublished drafts: all (omit key/keys/routes), one content key (key), or a selection (keys, routes). Destructive — check get_draft…`
- `edit_page`: `Open the interactive page canvas to change content: the user clicks an element, then you call patch_content. Use when the intent is editing…`
- `estimate_test`: `Estimate days to reach promote readiness for a page (traffic baseline). Read-only.`
- `find_replace`: `Case-insensitive find→replace across pages in one staged commit. Batch all replacements into ONE call — never parallelize find_replace on t…`
- `get_account_context`: `Account, user, memberships[]. Pass workspace on writes when memberships.length > 1.`
- `get_activity`: `List site activity or fetch one change diff (pass id). Filters: who, state, actor (me), since, limit≤20. Notes from context are visible to…`
- `get_adapt_status`: `Read adapt state: proposal summary + proposalEtag (+ applied/consumed flag), undo-record presence, active or queued job progress. Use to re…`
- `get_analytics`: `Read-only traffic overview (default) or full breakdowns via include[]; optional bot id for crawler page drill-down.`
- `get_asset`: `Read one asset (metadata + base64 + stored sha256). sha256 is the stored blob; may differ from upload bodySha256 when IMAGES re-encodes ras…`
- `get_content`: `Read one content key; optional selector (region) or published=true (live body). Bodies over 40KB without a selector return a truncated summ…`
- `get_custom_domain_connect`: `Current connect session and nextAction (browser URL or manual DNS guide).`
- `get_draft_status`: `Pending draft changes: content keys and routes with status. May include requiredDecision (publish_confirm) before publish_site.`
- `get_form_submission`: `Read one form submission with the full field payload (explicit PII access — use only when needed).`
- `get_menu`: `Read a menu's draft items and etag; menu rules → get_skill('nav').`
- `get_menu_doc`: `Read the whole menu doc (all menus + shell/template), etag for put_menu_doc, and issues (by item id) — page_not_routable, page_missing, pag…`
- `get_route`: `Get one route by path (home is '/').`
- `get_site`: `Site detail, stats, publicUrl, brief head (default-on), and readiness flags. pages[] is a ~25-entry head by default (stats.pages has the tr…`
- `get_site_build_progress`: `Read-only build progress for humans (build-theater view) during structure/adapt or after import. Agent reads structuredContent.forHumans —…`
- `get_site_manifest`: `Content keys + hashes only (optional routes=true) — static files live in list_assets, not manifest. Diff keys+hashes before apply_changeset…`
- `get_site_outline`: `Site shape: every layout and shared section ('sections': fragments/* by name, with page count, whether the file exists and staged-change fl…`
- `get_skill`: `Skill body + optional questions[]. Accepts an id OR a synonym (e.g. 'list', 'menu') — resolves aliases and suggests near-misses. Start with…`
- `get_structure_result`: `Last structure apply job result (structuredKeys, conflicts, partial).`
- `get_structure_status`: `Flat vs structured page counts; informs user — do not auto-run analyze/apply while requiredDecision pending.`
- `graduate_site`: `Enable site search & collections (kv → do-sqlite), one-way. Unlocks search_content, collection indexes, visitor /__paige/search, and moves…`
- `import_site_from_url`: `Import URL to draft. On complete, response may include requiredDecision — preview then ask mirror vs editable before structure_*.`
- `inspect_collection`: `Collection state — count, server.mode, sample entries, tag (membershipKind, match=) when discovered; plus name, noun, URL pattern, layout,…`
- `list_assets`: `CMS uploads under assets/ only — not mirrored clone CDN (get_site mirroredAssets or import warmJob). Not content — use list_content. Upload…`
- `list_collections`: `Collections on the site — name, noun, item count (or 'not published yet'), URL pattern, and whether any member is staged. Includes a collec…`
- `list_content`: `List content keys (HTML/md); not assets — use list_assets. Defaults to 50 keys per page — raise limit (max 1000) or pass cursor (from nextC…`
- `list_custom_domains`: `List all custom hostnames and connection status for the site.`
- `list_form_submissions`: `List form submissions (metadata + bounded field preview — not full PII). Works on kv and do-sqlite backends.`
- `list_goals`: `List site conversion goals (pageview paths and form submits). Required before start_test.`
- `list_my_sites`: `List your Dotsy sites. Renders a site-picker for humans; agent reads structuredContent. Use to choose a site — not for editing content (use…`
- `list_pages`: `List pages on a site — route settings (path/title/navLabel/purpose) by default, one row per route. Renders a page-picker for humans (redire…`
- `list_skills`: `Paige build skills (id + whenToUse). Pull get_skill on demand — do not duplicate in tool text.`
- `new_post_template`: `Read-only scaffold for a new post — suggested key/path, membership meta, blank or duplicate body. Then put_post (+ optional put_route).`
- `patch_content`: `Edit one content key via ops[] (selector ops or replace-string). Stages draft; op shapes in schema.`
- `patch_route`: `Partial route update (only sent fields change; an OMITTED field is left alone). On a field that accepts null (contentKey, redirectTo, redir…`
- `preflight_site`: `Plan check before publish or large build (counts, route soft limit, seo suggestions). When ok is false, blocking lists the failed suggestio…`
- `preview_page`: `Verify-only composed HTML check; home preview may include requiredDecision — ask mirror vs editable before structure_*.`
- `promote_experiment`: `Promote a winning A/B variant to live — explicit user instruction only; see get_skill('verify') § A/B.`
- `publish_site`: `Publish draft to live. feedback and handoff required (use dummy feedback + one-line handoff if clean).`
- and 31 more in [d4adb947e2c6cbd354fa.json](d4adb947e2c6cbd354fa.json)

## Changes

- 2026-10-13: [description changed, schema changed](../../deltas/2026-10-13/d4adb947e2c6cbd354fa.json): `6 field(s) changed; signals: length_more_than_doubled`
- 2026-10-11: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-11/d4adb947e2c6cbd354fa.json): `2 tool(s) added; 9 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.dotsy.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
