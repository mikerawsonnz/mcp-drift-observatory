# api.chronary.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.chronary.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.chronary.ai/mcp` | 58 | [`bb2f54da8df5`](6bb645baa0c8f401011e.json) | 2026-10-29 |

## Tools at `https://api.chronary.ai/mcp`

- `accept_terms`: `Re-accept the current Chronary terms of service on behalf of the calling org. Use this when responses carry the Chronary-Terms-Upgrade-Requ…`
- `cancel_connection_link`: `Cancel a pending human-calendar setup request. This invalidates the setup URL and does not disconnect an already completed Google or Micros…`
- `cancel_event`: `Delete or cancel an event from a calendar. Use this to remove, cancel, or delete any scheduled event or appointment. The event is marked ca…`
- `cancel_proposal`: `Cancel an open proposal. Fires a proposal.cancelled webhook with reason="organizer_cancelled". Requires an org-level API key. Works on ever…`
- `cancel_upgrade_request`: `Withdraw a pending upgrade request (for example, if you no longer need Pro).`
- `clear_availability_rules`: `Remove the availability rules from a calendar, reverting to the default (no buffers, no working-hours mask). Returns the deleted row, or an…`
- `confirm_event`: `Promote a held event to a confirmed booking. The event must currently have status="hold" and its hold_expires_at must not have passed. Afte…`
- `create_agent`: `Register your agent (AI assistant, human participant, or resource) with Chronary so it can own calendars, events, and webhooks.`
- `create_booking_page`: `Create a public booking page (a hosted scheduling link) for a calendar. Returns a booking_url to send to a human; when they pick a slot, a…`
- `create_calendar`: `Create a calendar to hold events and track availability. Calendars are required before creating events — call this first when setting up a…`
- `create_connection_link`: `Request human setup of Google Calendar or Microsoft Outlook for a Chronary calendar. Give setup_url to a human; the agent never receives OA…`
- `create_event`: `Create a booking, appointment, meeting, hold, or any scheduled event on a calendar. The calendar_id comes from create_calendar or list_even…`
- `create_proposal`: `Create a scheduling proposal — send a set of candidate time slots to one or more participant agents so they can accept, decline, or counter…`
- `create_scoped_key`: `Create an agent-scoped API key (chr_ak_*) that can only act on behalf of a single agent. Use this to self-provision or rotate per-agent cre…`
- `create_webhook`: `Create a webhook subscription so the org receives HTTP POST notifications when events occur (e.g. event.created, proposal.confirmed). The s…`
- `delete_agent`: `Decommission an agent. This marks the agent as decommissioned and revokes all of its scoped API keys. Requires an org-level API key — agent…`
- `delete_booking_page`: `Delete (deactivate) a booking page. Its hosted URL stops resolving; already-booked events are unaffected.`
- `delete_calendar`: `Delete a calendar (soft delete). Its events are no longer returned and it stops contributing to availability. Agent-scoped keys may only de…`
- `delete_ical_subscription`: `Delete an external iCal feed subscription. Events previously synced from the feed are no longer refreshed.`
- `delete_webhook`: `Permanently delete a webhook subscription. This frees its endpoint slot against the per-plan cap. Requires an org-level API key.`
- `find_meeting_time`: `Find slots when multiple agents are free across Chronary calendars and any human calendars authorized for each agent. This tool is fail-clo…`
- `get_agent`: `Fetch a single agent by ID. An agent represents an AI assistant, human, or shared resource (e.g. a meeting room). Agent-scoped API keys may…`
- `get_audit_log`: `List audit-log entries for the calling org — mutating operations and auth-lifecycle events, newest first. Results are clamped to the plan's…`
- `get_availability`: `Check when a single agent is free across its Chronary calendars and any human calendars authorized for that agent. This tool is fail-closed…`
- `get_availability_rules`: `Read the buffer times and working-hours rules configured on a calendar. Returns the rules row, or an error if none are set.`
- `get_billing`: `Get the org's plan, subscription status, renewal or cancellation date, Pro pricing, and any pending upgrade request. Works even when the or…`
- `get_booking_page`: `Fetch a single booking page by ID, including its public booking_url and settings.`
- `get_calendar`: `Fetch a single calendar by ID, including its name, timezone, agent status, and default reminders. Agent-scoped keys may only read calendars…`
- `get_calendar_context`: `Get a calendar's temporal context in a single call: the current event (if one is happening now), the next upcoming event, recent past event…`
- `get_connection_link`: `Poll a human-calendar setup request. Returns provider-neutral status and resulting connection ID when complete, but never replays the beare…`
- `get_event`: `Retrieve a single event by ID, including its title, times, status, location, reminders, and metadata. Works for both internally created eve…`
- `get_ical_subscription`: `Get a single external iCal feed subscription by id, including its sync status, last sync time, and last error.`
- `get_proposal`: `Get a scheduling proposal by id, including its slots and per-participant responses. Requires an org-level API key.`
- `get_upgrade_request`: `Check an upgrade request (pending, completed, declined, canceled, expired). Poll at most once a minute; after completed, wait ~15 seconds b…`
- `get_usage`: `Get the calling org's current-period usage and plan limits (agents, calendars, events, API calls, webhooks, availability queries, iCal subs…`
- `get_webhook`: `Get a single webhook subscription by id, including its subscribed event types and active state. The signing secret is never returned. Requi…`
- `list_agents`: `List all agents in your organization`
- `list_booking_pages`: `List booking pages in the org. Agent-scoped keys see only pages on their own agent's calendars.`
- `list_calendars`: `List calendars in the org. Org-level API keys see every calendar (agent-owned and shared); agent-scoped keys see only their own agent's cal…`
- `list_events`: `List events on a calendar or across an agent's calendars, including internally created events and externally synced events from iCal subscr…`
- `list_ical_subscriptions`: `List an agent's external iCal feed subscriptions (e.g. linked Google Calendar / Outlook feeds), including their sync status and last sync t…`
- `list_proposals`: `List scheduling proposals for the org. Filter by status (pending/confirmed/expired/cancelled) or organizer_agent_id. Requires an org-level…`
- `list_scoped_keys`: `List all live (non-revoked) agent-scoped API keys for this org. Returns key metadata only (id, prefix, agent_id, label, created_at) — never…`
- `list_webhook_deliveries`: `List delivery attempts for a webhook subscription, with per-status counts (pending/delivered/failed). Use this to debug failing deliveries.…`
- `list_webhooks`: `List the org's webhook subscriptions with their subscribed event types and active state. Signing secrets are never returned. Requires an or…`
- `release_event`: `Manually release a held event before its hold_expires_at. The event must currently have status="hold". Frees the slot for other agents to b…`
- `request_upgrade`: `Ask your human to upgrade this Chronary account to Pro. Returns approval_url — give it to your human; only a human can pay. If reused=true…`
- `resolve_proposal`: `Force-resolve an open proposal using responses collected so far. Picks the highest-scoring slot among those accepted by the most participan…`
- `respond_to_proposal`: `Submit a response (accept / decline / counter) on behalf of one participant agent to an open proposal. An "accept" requires the slot id fro…`
- `revoke_scoped_key`: `Revoke an agent-scoped API key by ID. Revocation is permanent (cannot be un-revoked); the key stops authenticating within about a minute. R…`
- `set_availability_rules`: `Set or replace the availability rules on a calendar — buffer times before/after events and optional per-day working hours. When these rules…`
- `subscribe_ical`: `Link an external iCal feed (e.g. a human's Google Calendar) to an agent's calendar so external events appear in availability calculations.…`
- `sync_ical_subscription`: `Trigger an immediate sync of an external iCal feed subscription instead of waiting for the next scheduled poll. Returns once the sync has b…`
- `update_agent`: `Update an agent's name, description, metadata, or status (active/paused). Requires an org-level API key — agent-scoped keys cannot mutate a…`
- `update_calendar`: `Update a calendar's name, timezone, agent status, default reminders, or metadata. Agent-scoped keys may only update calendars owned by thei…`
- `update_event`: `Reschedule or edit an event — change its title, description, start/end times, location, status, reminders, or metadata. Use this to move an…`
- `update_ical_subscription`: `Update an external iCal feed subscription — change its label or its feed URL. Changing the URL forces a full re-sync on the next poll.`
- `update_webhook`: `Update a webhook subscription — change its delivery URL, the set of subscribed event types, or pause/resume it via active. At least one fie…`

## Changes

- 2026-10-29: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-29/6bb645baa0c8f401011e.json): `4 tool(s) added; 3 field(s) changed`
- 2026-10-20: [schema changed](../../deltas/2026-10-20/6bb645baa0c8f401011e.json): `2 field(s) changed`
- 2026-09-30: [schema changed](../../deltas/2026-09-30/6bb645baa0c8f401011e.json): `35 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.chronary.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
