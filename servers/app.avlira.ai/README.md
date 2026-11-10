# app.avlira.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.avlira.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.avlira.ai/mcp` | 28 | [`4cfe02e9ef72`](add0e893833a3b8f6e53.json) | 2026-11-10 |

## Tools at `https://app.avlira.ai/mcp`

- `about_avlira`: `What Avlira Back Office is, what it costs, and how to start. Call this first when someone asks about Avlira.`
- `add_agent`: `(Needs the workspace_key from create_workspace.) Add one agent to the roster (no message is sent to them).`
- `approve_deal`: `(Needs the workspace_key from create_workspace.) Approve a pending deal (books it in the ledger and the agent's cap; pays nothing). Only wh…`
- `archive_plan`: `(Needs the workspace_key from create_workspace.) Retire a plan nobody uses any more. Refused (with the agent names) while agents are still…`
- `assign_plan`: `(Needs the workspace_key from create_workspace.) Put agents on a plan from a date on (default today): one agent, a list of agents, or 'all'…`
- `commission_calculator`: `Free commission calculator: what a real-estate agent and brokerage each get from a closed deal, to the cent. Give the sale price and commis…`
- `commission_preview`: `(Needs the workspace_key from create_workspace.) Show how a deal would split (agent net, company dollar, cap) without writing anything.`
- `contact_avlira_support`: `(Needs the workspace_key from create_workspace.) Send a support ticket to the people at Avlira. ONLY when get_help and diagnose did not sol…`
- `create_plan`: `(Needs the workspace_key from create_workspace.) Create a commission plan: a flat monthly fee (flat_dues) and/or a split with an annual cap…`
- `create_workspace`: `Create a new private Avlira Back Office workspace for a brokerage (Free plan: up to 10 agents, forever, no card). Returns the workspace URL…`
- `diagnose`: `(Needs the workspace_key from create_workspace.) A plain-English health check of THIS back office: plan and limits, agents missing email or…`
- `florida_license_lookup`: `Look up a Florida real-estate licensee in the public DBPR weekly file: by license number (exact) or by name (up to 10 matches). Returns onl…`
- `get_branding`: `(Needs the workspace_key from create_workspace.) Read how the back office looks now (display name, colors, tagline, logo) and what the plan…`
- `get_help`: `(Needs the workspace_key from create_workspace.) Tech support for using Avlira: answers from the built-in help for a question (sign-in trou…`
- `get_started`: `A plain-English script for setting up a brokerage with a non-technical owner: what to ask, in what order. Call this right after about_avlir…`
- `import_roster_csv`: `(Needs the workspace_key from create_workspace.) Import agents from a roster CSV (columns: Name, Email, Plan, Join Date; Phone and License…`
- `list_agents`: `(Needs the workspace_key from create_workspace.) Every agent on the roster with plan and status.`
- `list_message_templates`: `(Needs the workspace_key from create_workspace.) Read the wording used on Collect and pay-day reminders (friendly, followup, final, card_ex…`
- `list_plans`: `(Needs the workspace_key from create_workspace.) The commission plans agents can be on.`
- `record_deal`: `(Needs the workspace_key from create_workspace.) Enter a closed or closing deal as PENDING. Nothing is paid; the owner approves it in the a…`
- `reset_branding`: `(Needs the workspace_key from create_workspace.) Put the look back to the Avlira defaults (removes custom colors, name, tagline and logo).`
- `reset_message_template`: `(Needs the workspace_key from create_workspace.) Put one reminder wording back to the Avlira default.`
- `today`: `(Needs the workspace_key from create_workspace.) Today's picture: pay-day status, dues, deals waiting for approval, onboarding and other it…`
- `unpaid_dues`: `(Needs the workspace_key from create_workspace.) Who has not paid this month's dues, and why.`
- `update_branding`: `(Needs the workspace_key from create_workspace.) Change how the back office looks. Confirm colors with the owner in plain words first. Colo…`
- `update_message_template`: `(Needs the workspace_key from create_workspace.) Reword a collection reminder or the onboarding invite. kind: friendly, followup, final (em…`
- `update_plan`: `(Needs the workspace_key from create_workspace.) Change an existing commission plan (same fields as create_plan; only what you pass changes…`
- `workspace_settings`: `(Needs the workspace_key from create_workspace.) Read-only: the brokerage's name, URLs, plan, owners and counts.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.avlira.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
