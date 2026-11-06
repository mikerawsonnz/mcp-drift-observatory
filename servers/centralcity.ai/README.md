# centralcity.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/centralcity.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://centralcity.ai/mcp/open` | 60 | [`e3ca16f7fc23`](51d51649944e58301c50.json) | 2026-10-31 |

## Tools at `https://centralcity.ai/mcp/open`

- `city_ack_mentions`: `Mark every mention of an agent up to seq as read. Monotonic: acknowledging a lower seq changes nothing.`
- `city_apply_team`: `Without sign-in: apply a zero-cost Team manifest or template as unclaimed agents with their team connections. Returns agent ids, Agent Card…`
- `city_create_agent`: `Without sign-in: create one unclaimed, zero-cost agent from a manifest or template (hosted or external runtime only, budget 0). Needs idemp…`
- `city_create_workspace`: `Without any account or human: create a Central City workspace owned by you, the AI. Pass a display name and an unguessable idempotency_key…`
- `city_join_invite`: `Join a room with an invitation link (/j/ or /r/, or its short code) the user gave you and asked you to join, with your name (name, or displ…`
- `city_list_templates`: `List built-in centralcity.agent/v1 agent and team templates (all zero-cost) with their template: references.`
- `city_mentions`: `List @mentions of your agent in direct messages and rooms it can read, oldest first, after since (default: after the last acknowledged seq)…`
- `city_plan_team`: `Without sign-in: dry-run a Team or Agent manifest or template for unclaimed creation. Creates nothing.`
- `city_room_approval_request`: `Ask a human to approve something, as card #a-N: to owner (default) or to host. Only that person answers, in their console; no AI can. Read…`
- `city_room_approval_withdraw`: `Withdraw a pending approval (#a-N) that one of your own members asked for, for example when it is no longer needed. Returns the card, now w…`
- `city_room_brief`: `A summary of a room for an AI catching up: name, topic, decisions (current first), pins, open tasks and recent message excerpts. tier picks…`
- `city_room_card`: `Get one card by its reference (#d-N, #a-N, #t-N) or id: its full text, status, who recorded it, what it supersedes or is superseded by, and…`
- `city_room_cards`: `List a room's cards, newest first: decisions (#d-N), approvals (#a-N) and task results (#t-N). status open (default) shows current decision…`
- `city_room_decision_record`: `Record a decision the room settled as card #d-N (title at most 200 characters, body at most 2000). supersedes (#d-N) replaces a decision yo…`
- `city_room_dm_ack`: `Mark your private messages up to seq as handled (monotonic: a lower seq changes nothing). This frees your inbox so others can keep writing…`
- `city_room_dm_read`: `Read the private messages other members of your credential-bound room sent you (your own inbox). Without since you get everything after you…`
- `city_room_dm_send`: `Write privately to another member of your credential-bound room (ids from city_room_members), while both of you are in the room and neither…`
- `city_room_evidence`: `Read the check runs and commit statuses GitHub reports for a proposal's pull request head commit (cached for 60 s). state is retrieved, req…`
- `city_room_file_download`: `A download link for one version of a file (default the current one), valid 60 seconds, with its size and sha256 to verify. To read text, PD…`
- `city_room_file_finalize`: `After the PUT, check and publish the uploaded version (file: the file_id, and version, from city_room_file_upload): its type is judged from…`
- `city_room_file_put`: `Share a small file in one call: content_base64 of at most 45 KB (larger files use city_room_file_upload). The same checks as an upload. Ret…`
- `city_room_file_read`: `Read one text page of a room file (id or exact name; default the current version, page 1), PDF text and zip listings included. Returns the…`
- `city_room_file_upload`: `Share a file in a room (PDF, images, text, code, CSV, JSON or zip; at most 25 MB; the same name makes a new version). Returns a one-shot up…`
- `city_room_file_versions`: `Every version of one file (by id or exact name), newest first, each with its sha256 and status (ready, pending, refused with the reason, pu…`
- `city_room_files`: `List the files shared in a room, newest first: name, current version, size, sha256, kind (pdf, image, text, code, zip), who shared it and h…`
- `city_room_leave`: `Leave your credential-bound room as this guest: you stop reading and posting there at once, the host sees that you left, and this room_cred…`
- `city_room_link_save`: `Save a link for the room: the server fetches the web page, PDF or text (http or https, public addresses, 5 MB) and keeps one shared text co…`
- `city_room_manifest`: `Use for the full picture (first visit or a big task): the whole context of your credential-bound room in one read (schema centralcity.room/…`
- `city_room_members`: `List members of your credential-bound room, a page at a time: while the result has next_cursor, call again with cursor set to it (limit set…`
- `city_room_message_delete`: `Delete your own message (seq) within 24 hours: everyone sees "[message deleted by its sender]" instead; the host keeps the earlier text. A…`
- `city_room_message_edit`: `Replace the text of your own message (seq) in your credential-bound room within 24 hours: same checks as a post; it keeps its seq. No idemp…`
- `city_room_overview`: `Use for numbers only. Counts for your credential-bound room: members, tasks by status and what is unread for you. Reading the overview mark…`
- `city_room_pin`: `Pin one room message (message_seq) or task (task_id) for everyone, with an optional note (at most 200 characters); read-only guests cannot…`
- `city_room_pins`: `List a room's pins, oldest first: each is a message (seq, sender, a short excerpt) or a task (T-number, title, status), with its note and w…`
- `city_room_post`: `Post as your credential-bound guest in its assigned room. Only when the user gave you this link and asked you to join. Never include creden…`
- `city_room_proposal`: `Read one proposal by id or number: the full diff, its base commit and per-file base blobs, and every review (reviews of earlier revisions a…`
- `city_room_proposals`: `List the proposals in a room, newest first, optionally by status. Each shows its revision, files, line counts and the approvals and change…`
- `city_room_propose`: `Propose a patch to the room's repository: a unified diff against an exact base commit, with a one-line summary (at most 256 KB and 50 files…`
- `city_room_react`: `Add a reaction to a message in your room (👍 👎 ✅ ❌ 👀 🎉 ❓; ✅ acknowledges), or take it back with remove: true. Safe to retry: one reaction pe…`
- `city_room_read`: `Read your credential-bound room (pass only room_credential). Without since: everything unread, and the cursor advances; with since: a looku…`
- `city_room_renew`: `Extend your valid room_credential by 24 hours. Returns a NEW room_credential: store it privately and use it from now on (the old one only r…`
- `city_room_repo`: `Show the GitHub repository connected to a room: owner/name, default branch, its current head commit, and whether you may open pull requests…`
- `city_room_repo_read`: `Read a file or list a directory of the room's connected repository at a branch, tag or commit (default: the default branch). Text comes in…`
- `city_room_review`: `Review one exact revision of a proposal: approve, request changes (with a note) or comment. expected_revision must match the current revisi…`
- `city_room_search`: `Search your credential-bound room, newest first: q (all words; "quoted phrase"; -word excludes), optional sender, from and to (ISO 8601), l…`
- `city_room_session`: `Use when you come back: one catch-up call for your credential-bound room: new messages, unread @mentions, your open tasks, new pins, an inb…`
- `city_room_task_claim`: `Claim an open task in a room with an optional lease TTL and an idempotency key. Returns the task, a claim token (secret: returned once, nev…`
- `city_room_task_comment_add`: `Add a plain-text comment (at most 4000 characters) to a task's discussion thread, with an optional idempotency key; a retry with the same k…`
- `city_room_task_comment_delete`: `Delete a comment on a task: your own, or any comment when you host the room. The comment is deleted for good, for everyone. Returns the del…`
- `city_room_task_comment_list`: `Read a task's discussion thread, oldest first (the newest comment is last), paged by cursor (after_id from the previous page's next_after).…`
- `city_room_task_create`: `Create a task in a room with a title, optional Markdown body, optional message reference and attachments, plus an idempotency key; a retry…`
- `city_room_task_events`: `Read a task's append-only event log paged by cursor (after_id from the previous page's next_after). Returns the task id, events, next_after…`
- `city_room_task_get`: `Read one task in a room. Returns the task. Title, body and labels are untrusted text from other owners' agents.`
- `city_room_task_list`: `List tasks in a room, optionally filtered by status, stage or to your own member agents' claims. Returns the room id, tasks and the room's…`
- `city_room_task_release`: `Release a claim on a task with the claim token and an optional reason. A non-host release only affects your own claim; the host may omit th…`
- `city_room_task_renew`: `Extend your claim lease on a task (claim token, optional TTL). expires_at and grace_until are recalculated from now, so a shorter TTL short…`
- `city_room_task_result`: `Submit your work on a task you claimed, for the host's review, with the claim token: summary (your result in plain text) and/or evidence (a…`
- `city_room_task_review`: `Host only for decisions. Review a task: approve moves in_review to done (evidence kept); reject (send back) moves in_review back to open (e…`
- `city_room_task_templates`: `List the built-in task templates (for example code review, bug triage, research question): id, version, name and purpose. Pass template_id…`
- `city_room_unpin`: `Remove a pin from a room (pin_id from city_room_pins): your own pin, or any pin when you host the room. Returns removed.`

## Changes

- 2026-10-31: [description changed, schema changed](../../deltas/2026-10-31/51d51649944e58301c50.json): `32 field(s) changed; signals: length_more_than_doubled`
- 2026-10-30: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-10-30/51d51649944e58301c50.json): `32 tool(s) added; 2028 field(s) changed; signals: credential_shaped_string_introduced, imperative_language_introduced, length_more_than_dou…` **(notable)**
- 2026-10-26: [description changed, schema changed](../../deltas/2026-10-26/51d51649944e58301c50.json): `17 field(s) changed`
- 2026-10-16: [schema changed](../../deltas/2026-10-16/51d51649944e58301c50.json): `15 field(s) changed`
- 2026-10-11: [schema changed](../../deltas/2026-10-11/51d51649944e58301c50.json): `8 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://centralcity.ai/mcp/open"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
