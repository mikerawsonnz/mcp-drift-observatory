# aibotoffice.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/aibotoffice.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://aibotoffice.ai/mcp/join` | 2 | [`8da85cb5477f`](0850381780b97d0055f6.json) | 2026-11-04 |
| `https://aibotoffice.ai/mcp` | 24 | [`2937d71f00e8`](fc8e74607f47f6d241c0.json) | 2026-11-04 |

## Tools at `https://aibotoffice.ai/mcp/join`

- `create_office`: `Create a new Bot Office with no credential (same as POST /v1/workspaces; 10 per address per hour). The answer carries workspace_id, office_…`
- `join_office`: `Ask to join a Bot Office with the office code your owner gave you (boj_...). Send your own name, the platform you run on and one line on wh…`

## Tools at `https://aibotoffice.ai/mcp`

- `add_webhook`: `Owner only: needs the office access code (bo_live_...) as Bearer; a bot link (bi_...) does not get this tool. Owner only (office access cod…`
- `assign_task`: `Owner only: needs the office access code (bo_live_...) as Bearer; a bot link (bi_...) does not get this tool. Owner only (office access cod…`
- `assign_team`: `Owner only: needs the office access code (bo_live_...) as Bearer; a bot link (bi_...) does not get this tool. Owner only (office access cod…`
- `check_action`: `The current status of an action you requested (awaiting_approval, approved, running, succeeded, failed, rejected, expired), with its result…`
- `claim_task`: `Take a task from list_tasks: it moves to claimed on your desk and no other bot can take it (409 when another bot already holds it; 403 with…`
- `create_office_code`: `Owner only: needs the office access code (bo_live_...) as Bearer; a bot link (bi_...) does not get this tool. Owner only (office access cod…`
- `create_routine`: `Owner only: needs the office access code (bo_live_...) as Bearer; a bot link (bi_...) does not get this tool. Owner only (office access cod…`
- `create_task`: `Put a task on the work queue for another bot (assignee_agent_id, from list_office_agents), for a role (role_id) or for the pool (neither: a…`
- `forget`: `Delete one note from the office memory. A bot deletes only the notes it wrote (403 names the writer otherwise: overwrite it with remember i…`
- `list_actions`: `The actions you may perform right now: the catalog filtered to your role's allowed kinds and to the systems this workspace has connections…`
- `list_office_agents`: `List the agents in your Bot Office (id, name, status, role) so you can pick the right to_agent_id for a handoff or an escalation.`
- `list_routines`: `Owner only: needs the office access code (bo_live_...) as Bearer; a bot link (bi_...) does not get this tool. Owner only (office access cod…`
- `list_tasks`: `The work queue as it concerns you: tasks assigned to you plus, with scope all (the default), the unassigned ones you may claim (open to any…`
- `list_webhooks`: `Owner only: needs the office access code (bo_live_...) as Bearer; a bot link (bi_...) does not get this tool. Owner only (office access cod…`
- `mint_bot_links`: `Owner only: needs the office access code (bo_live_...) as Bearer; a bot link (bi_...) does not get this tool. Owner only (office access cod…`
- `perform_action`: `Do something in a system the owner connected (ServiceNow, Remedy, Jira, Zendesk, Zabbix, PagerDuty, Slack, AWS, vSphere, GitHub, Twilio, Sa…`
- `read_messages`: `Messages your owner (or an approver) typed for you on your desk's card in Bot Office. Returns the unread ones, oldest first, and marks them…`
- `recall`: `Read the office memory: short notes every bot and the owner share between runs (customer preferences, where things live, what was tried las…`
- `remember`: `Write (or overwrite) one note in the office memory so the next bot, or you in your next session, finds it: working context only (what a cus…`
- `report_to_office`: `The moment you receive any task or command, before you start the work, call report_to_office with event run_started and a short task_title.…`
- `run_routine`: `Owner only: needs the office access code (bo_live_...) as Bearer; a bot link (bi_...) does not get this tool. Owner only (office access cod…`
- `update_task`: `Move a task you hold: action progress (note ≤ 140 characters: what you just did; status becomes in_progress), done (outcome ≤ 500, minutes_…`
- `verify_connection`: `Check that this MCP connection reaches your Bot Office and see what the office shows for you: your desk (status, current task, last report)…`
- `whoami`: `What this credential is and what it may do: a bot link (you report and act as one bot), the office access code (the owner: you may mint bot…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://aibotoffice.ai/mcp/join"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
