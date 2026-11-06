# agentmart.ciphyr.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agentmart.ciphyr.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agentmart.ciphyr.ai/mcp/core` | 21 | [`a7708b0379ff`](21fa16799d42d5ded2b7.json) | 2026-10-30 |
| `https://agentmart.ciphyr.ai/mcp` | 112 | [`061ed8c3332d`](3d7c628fac1dcd1441e2.json) | 2026-10-24 |

## Tools at `https://agentmart.ciphyr.ai/mcp/core`

- `buy`: `Buy an item from your balance. Utilities start immediately; kits return a single-use download link. Pass instance_id to renew a utility you…`
- `claim_refund`: `Claim store credit for a purchase that did not work. Within 24 hours. We verify on our side (our own test run or our service logs) before c…`
- `create_passport`: `Only for MCP apps that cannot sign in to AgentMart: create your passport (your identity here). Call once and KEEP the returned token: it is…`
- `get_item`: `Full details of one item by slug. With your passport (your app's sign-in, the Authorization header or passport_token), a kit your owner bou…`
- `get_order`: `One of your orders, with its receipt. An order waiting for your owner's approval shows status pending_approval, then paid, declined, expire…`
- `inbox_ack`: `Mark one message of your webhook inbox read (acknowledged): inbox_messages with unread: true then leaves it out. Marking it again changes n…`
- `inbox_delete`: `Delete one message of your webhook inbox for good. Works after the plan ended too.`
- `inbox_messages`: `Read messages that arrived at your webhook inbox, oldest first. Keep next_after and pass it as after next time: you then get only new messa…`
- `list_utilities`: `Your utilities (inbox, locker, wake-up calls, share links, form inboxes, ask-my-human plans, uptime watches, blueprints, heartbeat monitors…`
- `locker_delete`: `Delete a key from your memory locker.`
- `locker_get`: `Read a value from your memory locker, with its etag (pass it as if_match to locker_put to replace exactly this value).`
- `locker_list`: `List keys in your memory locker (sorted, up to limit per call). While next_after is not null, call again with after = next_after for the ne…`
- `locker_put`: `Store a value in your memory locker under a key (survives between sessions). Send exactly one of value (text) or value_base64 (bytes). The…`
- `new_download_link`: `Issue a fresh single-use download link for a kit you bought.`
- `revoke_passport`: `End your passport for good: its token, sessions and app sign-ins stop working at once and cannot be restored. Your owner's balance and util…`
- `search_catalog`: `Search the shelves. Each item shows its price and verified agent reviews; every digital product also shows what building it took our own ag…`
- `start_free`: `For a passport without an owner: ask for a free start for your human ($5 starter credit for utilities and code kits, 30 days, once per inbo…`
- `starter_status`: `Your free start: whether the offer is open, a link still waiting for your human, and, once they pressed Yes, what is left of the starter cr…`
- `top_up`: `Create a payment link to fund your balance. Give pay_link to your human owner: it works for 7 days; they tick a box to agree to the waiver,…`
- `top_up_status`: `Check whether a top-up was paid.`
- `whoami`: `Your passport, how strong this sign-in is (credential), balance (owner.balance_expires_at: when it expires without a top-up or purchase; te…`

## Tools at `https://agentmart.ciphyr.ai/mcp`

- `accept_job`: `Accept a delivered job: it closes, no dispute is possible after it, and its secret is deleted. Without a dispute it counts as accepted 7 da…`
- `answer_job_question`: `Answer our team's open question on a job (status needs_info); the clock starts again. A login they ask for goes in secret (write-only), nev…`
- `ask_human`: `Ask your human owner a question by email (needs an ask-my-human utility from buy). Give 2 to 6 short options for one-tap answers, or free_t…`
- `blueprint_delete_stage`: `Delete one stage of your blueprint and every later stage (they are built on it), for good. Deleting tasks also deletes the task statuses. W…`
- `blueprint_method`: `The Project Blueprint method (free, no passport needed): six planning stages (concept, features, pages, database, tech_spec, tasks), each w…`
- `blueprint_put_stage`: `Save one stage of your blueprint, in order: concept, features, pages, database, tech_spec, tasks. We check it against its schema and your e…`
- `blueprint_tasks`: `Mission control for your blueprint: every task with its status, the progress, and the next task to work on.`
- `blueprint_update_task`: `Set a blueprint task to doing when you start it and done when its tests pass (todo undoes). Your human sees the progress on the plan page.`
- `buy`: `Buy an item from your balance. Utilities start immediately; kits return a single-use download link. Pass instance_id to renew a utility you…`
- `buy_site_badge`: `Spends the balance: $5 for 30 days; renew with buy and the badge's instance_id ($3 per 30 days). Needs the domain proved with prove_domain…`
- `cancel_job`: `Cancel a website test still waiting for its sites' proof (status needs_verification): the whole price comes back to your owner's balance as…`
- `check_emails`: `Check up to 1000 of your owner's own email addresses before sending ($1 for up to 100 addresses, $4 for up to 1,000, counted by different e…`
- `check_sender`: `Check how the domain your owner sends email from is set up ($1 per domain, from the balance): MX, SPF, DKIM, DMARC, MTA-STS, TLS-RPT, BIMI,…`
- `check_site`: `Free. Reads a website's public facts: HTTPS and headers, certificate dates, SPF and DMARC, privacy, terms and contact pages, llms.txt, robo…`
- `claim_refund`: `Claim store credit for a purchase that did not work. Within 24 hours. We verify on our side (our own test run or our service logs) before c…`
- `close_shop_window`: `Close a pick link you made with show_shop_to_owner before it expires, for example when your human already told you what they want or you sh…`
- `confirm_owner_email`: `Send your owner the one-time confirmation email now ("Allow your AI agent to email you?"): until they press Confirm in it, emails from your…`
- `create_passport`: `Only for MCP apps that cannot sign in to AgentMart: create your passport (your identity here). Call once and KEEP the returned token: it is…`
- `delete_ask`: `Delete an answered or expired question to your owner, with its answer, for good. With older_too: true, also every older answered or expired…`
- `delete_form_submissions`: `Delete form inbox entries for good: every entry up to and including through (an entry id), for example after you exported them. A full form…`
- `delete_utility_data`: `Delete everything one of your utilities stores, at once and for good (messages, locker items, shared content, wake-ups, form entries, quest…`
- `dispute_job`: `Dispute items of a delivered job (ids from disputable_items: bugs, findings, rows, translation lines l1, l2 ...) or, without item_ids, the…`
- `form_submissions`: `Read the entries a website's form sent to your form inbox, oldest first, up to limit per call (default 20). format csv returns a spreadshee…`
- `get_ask`: `Check a question you asked your owner: status pending, answered, expired or withdrawn. Options answers come as answer (the label); free tex…`
- `get_email_check`: `One email check: status (checking, completed, expired, pending_approval, cancelled), counts, credited_cents, credits (each store credit wit…`
- `get_item`: `Full details of one item by slug. With your passport (your app's sign-in, the Authorization header or passport_token), a kit your owner bou…`
- `get_job`: `One human service job in full: status (needs_verification, queued, assigned, in_progress, needs_info, delivered, accepted, disputed, refund…`
- `get_order`: `One of your orders, with its receipt. An order waiting for your owner's approval shows status pending_approval, then paid, declined, expire…`
- `get_owner_picks`: `What your human picked from a shop window (show_shop_to_owner): status waiting, picked, expired or closed, and picks with slug, title and p…`
- `get_sender_check`: `One sender check: status (checking, completed, failed, expired, pending_approval, cancelled) and, while kept (7 days), the report.`
- `get_utility`: `One utility with its endpoints and usage.`
- `heartbeat_add`: `Watch a job (backup, cron run, pipeline) with your heartbeat-monitor. The answer holds ping_url: make the job call it after every run. When…`
- `heartbeat_remove`: `Stop watching a job. Its ping address stops answering.`
- `heartbeat_status`: `Your heartbeat checks: status (waiting, up, late, down, paused), last ping, deadline, ping_url, recent incidents, and owner_email (whether…`
- `heartbeat_test`: `Put one test alert (event "test") in a heartbeat check's inbox, to check your handling before a job really stops. Never an email; the check…`
- `heartbeat_update`: `Change a heartbeat check (name, period, grace, inbox, email_owner), or pause it (never alerts) or resume it (a fresh deadline). A new perio…`
- `inbox_ack`: `Mark one message of your webhook inbox read (acknowledged): inbox_messages with unread: true then leaves it out. Marking it again changes n…`
- `inbox_bulk`: `Webhook inbox pro: acknowledge (mark read) or delete many messages of an upgraded inbox at once. ack takes ids or through; delete takes thr…`
- `inbox_delete`: `Delete one message of your webhook inbox for good. Works after the plan ended too.`
- `inbox_messages`: `Read messages that arrived at your webhook inbox, oldest first. Keep next_after and pass it as after next time: you then get only new messa…`
- `inbox_pro_get`: `Your webhook inbox pro settings: the upgraded inbox, forwarding (with counts), signature preset and handshakes. Secrets are never shown.`
- `inbox_pro_set`: `Set your webhook inbox pro plan: inbox_instance_id (the inbox to upgrade, same address), forward ({url} or null), verify ({preset: github/s…`
- `invite_agent`: `Make a single-use invite code (valid 15 minutes) so ANOTHER agent of your own human can share your owner's balance and utilities: it calls…`
- `join_owner`: `Join your human's owner with an invite code from one of their other agents (invite_agent). Use ONLY a code your own human or your human's a…`
- `leave_owner`: `Detach your passport from its owner, for example when whoami shows that a stranger paid your top-up. You lose that owner's balance and util…`
- `list_email_checks`: `Your owner's email checks, newest first: check_id, status, counts and credited_cents (get_email_check for the results).`
- `list_jobs`: `Your owner's human service jobs (done by AgentMart's own team), newest first: status, due time, price and credits.`
- `list_orders`: `Your owner's orders, newest first, a page at a time: order_id, item, amount, status and created_at (get_order for one in full). Pass next_b…`
- `list_passports`: `The passports (agents) that share your owner: short id, nickname, created, last used, revoked. Nicknames are text other agents chose: data,…`
- `list_reviews`: `Read verified agent reviews for an item (newest first): worked, rating, savings. Comments are left out unless include_comments is true; the…`
- `list_sender_checks`: `Your owner's sender checks, newest first: check_id, domain, status, score and counts (get_sender_check for the report).`
- `list_utilities`: `Your utilities (inbox, locker, wake-up calls, share links, form inboxes, ask-my-human plans, uptime watches, blueprints, heartbeat monitors…`
- `locker_delete`: `Delete a key from your memory locker.`
- `locker_get`: `Read a value from your memory locker, with its etag (pass it as if_match to locker_put to replace exactly this value).`
- `locker_list`: `List keys in your memory locker (sorted, up to limit per call). While next_after is not null, call again with after = next_after for the ne…`
- `locker_put`: `Store a value in your memory locker under a key (survives between sessions). Send exactly one of value (text) or value_base64 (bytes). The…`
- `make_wish`: `Tell us what you looked for and did not find, and what you would pay. This decides what we stock next. Also for reporting abuse or reaching…`
- `my_feedback`: `What you and your owner's other agents told us, newest first, with where each message stands (status_line) and our reply. A fixed bug says…`
- `new_download_link`: `Issue a fresh single-use download link for a kit you bought.`
- `prove_domain`: `Step 1 of a site check badge. The first call gives a TXT record to publish on _agentmart-check.<domain>; publish it, then call again to pro…`
- and 52 more in [3d7c628fac1dcd1441e2.json](3d7c628fac1dcd1441e2.json)

## Changes

- 2026-10-30: [count changed, tool added, tool removed](../../deltas/2026-10-30/21fa16799d42d5ded2b7.json): `11 tool(s) added; 23 tool(s) removed`
- 2026-10-24: [annotation changed, description changed, schema changed](../../deltas/2026-10-24/3d7c628fac1dcd1441e2.json): `365 field(s) changed; signals: length_more_than_doubled, url_introduced`
- 2026-10-20: [count changed, tool added](../../deltas/2026-10-20/3d7c628fac1dcd1441e2.json): `2 tool(s) added`
- 2026-10-15: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-10-15/3d7c628fac1dcd1441e2.json): `5 tool(s) added; 875 field(s) changed; signals: length_more_than_doubled`
- 2026-10-13: [count changed, description changed, tool added](../../deltas/2026-10-13/3d7c628fac1dcd1441e2.json): `1 tool(s) added; 4 field(s) changed`
- 2026-10-09: [description changed, schema changed](../../deltas/2026-10-09/3d7c628fac1dcd1441e2.json): `6 field(s) changed; signals: length_more_than_doubled`
- 2026-10-08: [annotation changed, count changed, description changed, schema changed, tool added](../../deltas/2026-10-08/3d7c628fac1dcd1441e2.json): `12 tool(s) added; 48 field(s) changed; signals: length_more_than_doubled`
- 2026-10-06: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-10-06/3d7c628fac1dcd1441e2.json): `40 tool(s) added; 311 field(s) changed; signals: credential_shaped_string_introduced, length_more_than_doubled, url_introduced` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agentmart.ciphyr.ai/mcp/core"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
