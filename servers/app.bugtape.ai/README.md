# app.bugtape.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.bugtape.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.bugtape.ai/demo/mcp` | 14 | [`806cedcfeac4`](9b7601666bc78c4330a2.json) | 2026-11-03 |

## Tools at `https://app.bugtape.ai/demo/mcp`

- `get_bug`: `Get full details of a bug including title, description, severity, status, reporters, AI summary, environment info, report count, affected_u…`
- `get_bug_events`: `Get session events for a bug (DOM, network, console, clicks, errors). Prefer passing occurrenceId so events are not mixed across captures.`
- `get_bug_history`: `Get the full audit trail of status/severity changes and assignments on a bug, including who changed what and when.`
- `get_bug_occurrences`: `List the individual occurrences grouped under a bug. Use this to see which users, sessions, releases, or environments were affected.`
- `get_bug_users`: `Who hit this bug: one row per affected end user (the app's identify() userId, else reporter email, else an anonymous IP-hash key) with firs…`
- `get_current_org`: `Return the credential workspace. Agent PATs resolve only their own workspace; human sessions use BUGTAPE_ORG_ID.`
- `get_live_occurrences`: `Get the most recent occurrences across the organization. Useful for live monitoring and tester workflows. Honors deliveryFeed (tool arg, el…`
- `get_project_stats`: `Get aggregate statistics for a project (server-computed over bugs in the elected delivery feed, not a sample): counts by status and severit…`
- `get_repro_context`: `Build an agent-consumable reproduction pack: evidence (timeline, status, env) separate from inference (AI summary). Prefer occurrenceId so…`
- `get_similar_bugs`: `Find other bugs similar to the given bug, ranked by similarity score (0-100, fingerprint + title overlap). Returns up to 5 matches. Useful…`
- `list_bug_groups`: `Grouped triage view: bugs collapsed across pages by error signature (one group per distinct error within a project, even when dedup created…`
- `list_bugs`: `List bugs for the organization (flat, one row per deduplicated report). Supports filtering by status, severity, project, platform, delivery…`
- `list_projects`: `List all projects in the organization with their bug counts.`
- `list_recommended_critical`: `Start here. Returns 'sentToYou' first: bugs a person sent you with "Send to agent" (fix these first), then the prefiltered agent inbox: one…`

## Changes

- 2026-11-03: [description changed](../../deltas/2026-11-03/9b7601666bc78c4330a2.json): `3 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.bugtape.ai/demo/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
