# finestructure.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/finestructure.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://finestructure.ai/api/mcp` | 93 | [`80020bc89dc3`](65e5013537444a3c6e16.json) | 2026-10-05 |

## Tools at `https://finestructure.ai/api/mcp`

- `add_custom_domain`: `Attach or replace the app custom domain through the same Fine Structure Studio custom-domain flow. Returns exact DNS verification and routi…`
- `add_file_change`: `Stage one file upsert or delete inside a change set. Does not modify the live app until apply_change_set. Paths follow the Fine Structure a…`
- `agency_create_claim_link`: `Agency mode only. Create a client claim link for an existing app owned by the agent. The client must log in with the invited email before o…`
- `agency_create_client`: `Agency mode only. Create or update a client record for an account-level agent. This does not create a verified Fine Structure user account…`
- `agency_create_client_app`: `Agency mode only. Create a new app owned by the agent, start generation, and create a claim link for the client. Ownership transfers only w…`
- `agency_get_claim_status`: `Agency mode only. Inspect one handoff status without exposing the raw claim token.`
- `agency_list_clients`: `Agency mode only. List client records and app handoff status for the authenticated agent.`
- `apply_change_set`: `Apply a staged change set to the app. Creates a Saved Version before applying. Blocks on validation errors unless force=true.`
- `attach_agent_whatsapp`: `Connect a platform WhatsApp number to one of the account's agents, so the owner can message that number and reach that agent. Requires the…`
- `check_domain_verification`: `Check Fine Structure custom-domain verification and SSL status for the configured custom domain, then save the latest status.`
- `check_subdomain_available`: `Check whether a platform subdomain can be claimed before calling set_app_subdomain. Returns available plus a status of available, invalid,…`
- `compare_current_to_version`: `Compare the current app files to a Saved Version and return compact per-file diffs.`
- `compare_saved_versions`: `Compare two Saved Versions and return per-file additions, removals, modifications, and compact diffs.`
- `configure_domain_redirects`: `Configure custom-domain redirect policy: primary domain, optional www/root redirect, and HTTPS enforcement.`
- `configure_integration`: `Store safe non-secret integration metadata for an app. Use set_secret for API keys/tokens.`
- `confirm_owner_phone_verification`: `Confirm the 6-digit code the owner received on WhatsApp from start_owner_phone_verification. On success the owner is verified: agents can m…`
- `create_ab_test`: `Create a native Fine Structure A/B test between existing app pages. Use update_app first if a variant page still needs to be generated. Cre…`
- `create_agent`: `Create an autonomous AI agent on the user's Fine Structure account: a standing worker, not a chat session. It gets the platform's default s…`
- `create_app`: `Create a new application from a natural language prompt. The AI generates a complete web app with pages, components, styling, and data mode…`
- `create_change_set`: `Create a staged file change set. Add multiple file changes, validate them as one app state, then apply atomically.`
- `create_entity_records`: `Create/insert records in one app entity. Executes directly for the authenticated app owner and returns the created record ids.`
- `create_entity_schema`: `Create an entity schema file in entities/<Entity>.json. Creates a Saved Version before writing.`
- `create_platform_request`: `Open a request to the Fine Structure platform team: a bug, a feature request or a question about the platform itself (not about the user's…`
- `delete_ab_test`: `Delete a native A/B test from an app. Creates a Saved Version before the change.`
- `delete_entity_records`: `Delete exact records by ID or exact-match filters. Executes directly for the authenticated app owner; pass expected_count as a safety check…`
- `delete_secret`: `Delete one app secret by key.`
- `detach_agent_whatsapp`: `Disconnect the owner's WhatsApp route from a platform number. Removes only this account's route; other accounts sharing the number keep the…`
- `discard_change_set`: `Discard a pending staged change set without changing app files.`
- `get_ab_test_stats`: `Get views, unique visitors, conversions, and conversion rates for an A/B test.`
- `get_agent_whatsapp`: `Read the WhatsApp state of the connected account: whether the owner's phone is verified, which platform numbers they can connect, and which…`
- `get_app_analytics`: `Traffic analytics for an app's published site over a chosen window: total views, unique visitors, daily series, top pages, top referrer dom…`
- `get_app_detail`: `Deep introspection of an app: entities, pages, settings, integrations, environment variables, and file structure. Use this to understand wh…`
- `get_app_files`: `Get the file tree for an app with paths and byte sizes.`
- `get_app_links`: `Return editor, preview, published path, subdomain, and custom-domain links plus whether each works for anonymous visitors, app users, or St…`
- `get_app_metadata`: `Read the saved public HTML-shell identity: name, description, language and image URLs/dimensions. Same settings as Studio SEO/GEO.`
- `get_app_security_audit`: `Read recent server-side security audit events for an app.`
- `get_app_security_context`: `Return safe security context for one owned app: owner id/email, Studio collaborators, generated-app members, route policies, entity policie…`
- `get_app_status`: `Get app overview: files, published state, URL, active jobs.`
- `get_domain_ssl_status`: `Return SSL/certificate status and pending certificate validation DNS records for the app custom domain.`
- `get_domain_verification`: `Return the exact DNS records and instructions required to verify and route the app custom domain.`
- `get_entities`: `Get all entity (data model) schemas for an app, with record counts. Each entity has fields, types, and relationships.`
- `get_errors`: `Get recent runtime errors for an app (last 20). Useful for diagnosing issues before updating.`
- `get_job_status`: `Poll the status of an async generation job. Use this after create_app or update_app to know when the job is done. Returns status ('running'…`
- `get_pages`: `Get all pages in an app with their file paths and sizes.`
- `get_platform_guide`: `Return a machine-readable Fine Structure / FSe2 guide for AI agents. Call this at the start of an MCP session to learn app files, entities,…`
- `get_platform_request`: `One platform request with its full history: team replies, status changes (open / triaged / in_progress / needs_info / deployed / wont_fix)…`
- `get_preview_url`: `Return editor preview and published/public URLs for an app.`
- `get_recommended_workflow`: `Return the recommended MCP tool sequence for a task type. Use this before creating apps, editing files, seeding data, publishing, setting u…`
- `inspect_preview`: `Return server-side preview context: URLs, persisted runtime/network errors, static clickable candidates, pages, and explicit live-browser a…`
- `invite_app_member`: `Provision a generated-app runtime member with a role. This does not create a Studio collaborator, and the owner role cannot be assigned. pa…`
- `invoke_function`: `Run a backend function of an owned app exactly like the HTTP route and return its status and JSON. caller='owner' runs as the app owner; ca…`
- `list_ab_tests`: `List the platform A/B tests configured for an app.`
- `list_agent_tasks`: `List scheduled tasks for one agent (or the whole account), including schedule, status and next_run_at.`
- `list_agents`: `List the AI agents on the user's account with id, name, role, status and FineMail address.`
- `list_app_domains`: `List an app's platform path, subdomain, and configured custom domain with verification, SSL, primary-domain, redirect, publish, and login-g…`
- `list_app_members`: `List generated-app runtime users/members for an app. This is separate from Studio project collaborators.`
- `list_apps`: `List applications owned by the authenticated user, newest activity first. Returns up to 'limit' apps per call plus the total count; page wi…`
- `list_integrations`: `List supported integrations and safe connected integration metadata for an app. Tokens/secrets are never returned.`
- `list_platform_requests`: `Your account's platform requests, newest activity first. Call it at the start of a session with since=<the updated_date you last saw> to le…`
- `list_saved_versions`: `List restorable Saved Versions for an app, including versions created by MCP writes.`
- and 33 more in [65e5013537444a3c6e16.json](65e5013537444a3c6e16.json)

## Changes

- 2026-10-05: [count changed, tool added](../../deltas/2026-10-05/65e5013537444a3c6e16.json): `2 tool(s) added`
- 2026-09-27: [count changed, description changed, schema changed, tool added](../../deltas/2026-09-27/65e5013537444a3c6e16.json): `7 tool(s) added; 29 field(s) changed; signals: credential_shaped_string_introduced, imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-09-26: [description changed, schema changed](../../deltas/2026-09-26/65e5013537444a3c6e16.json): `32 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-09-01: [count changed, tool added](../../deltas/2026-09-01/65e5013537444a3c6e16.json): `2 tool(s) added; signals: imperative_language_introduced` **(notable)**
- 2026-08-24: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-08-24/65e5013537444a3c6e16.json): `588 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://finestructure.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
