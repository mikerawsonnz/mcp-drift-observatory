# api.daystruct.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.daystruct.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.daystruct.ai/mcp` | 25 | [`88a77f8b6e7f`](e5ff8779bfb56c541392.json) | 2026-10-15 |

## Tools at `https://api.daystruct.ai/mcp`

- `answer_software_questions`: `Deprecated: this evidence tool is no longer refreshed and will be removed on or after 2026-12-31. For building, use discover_daystruct_capa…`
- `check_release_support`: `Deprecated: this evidence tool is no longer refreshed and will be removed on or after 2026-12-31. For building, use discover_daystruct_capa…`
- `check_security_exposure`: `Deprecated: this evidence tool is no longer refreshed and will be removed on or after 2026-12-31. For building, use discover_daystruct_capa…`
- `close_task_session`: `Close a task with its reported outcome and compact summary.`
- `compat_check`: `Resolve Daystruct capabilities to exact versions that fit each other, or get the exact constraint that broke with suggested alternatives. S…`
- `create_task_session`: `Start compact task context with optional capability steps and dependencies. Requires read and requests:write. No conversation or reasoning…`
- `daystruct_status`: `Read the public Daystruct manifest: how capabilities are discovered, checked for compatibility and delivered.`
- `discover_daystruct_capabilities`: `Browse every public Daystruct capability without an account, or search using a task sentence or tool name. Lists default to eight compact d…`
- `get_compat_verify_kit`: `Return the files of the local verify step for exact source members from compat_check: a script, its plan, and the interface conformance sui…`
- `get_context_contract`: `Deprecated: this evidence tool is no longer refreshed and will be removed on or after 2026-12-31. For building, use discover_daystruct_capa…`
- `get_daystruct_account`: `Read the connected key's account: available and reserved credits, the key's scopes, its per-call spending limit (null means none) and where…`
- `get_daystruct_validated_guidance`: `Retrieve reviewed Frontier guidance scoped to an exact databank, task family and tested model. Returns only live, unexpired promotions and…`
- `get_entity_evidence`: `Deprecated: this evidence tool is no longer refreshed and will be removed on or after 2026-12-31. For building, use discover_daystruct_capa…`
- `get_task_session`: `Read compact task context or preview the next ready capabilities without consuming them or extending the session TTL.`
- `list_daystruct_guidance_scopes`: `Find task families and exact tested models with live Frontier guidance for a databank, before requesting that guidance.`
- `lookup_vulnerability`: `Deprecated: this evidence tool is no longer refreshed and will be removed on or after 2026-12-31. For building, use discover_daystruct_capa…`
- `plan_project_development`: `Get a small stage-specific capability selection and concrete next actions from a caller-approved project projection. Keep source and full s…`
- `prepare_daystruct_capabilities`: `Group up to six discovered capability IDs into a plan with each profile and delivery instructions. Missing entries remain explicit. Does no…`
- `read_recent_evidence_changes`: `Deprecated: this evidence tool is no longer refreshed and will be removed on or after 2026-12-31. For building, use discover_daystruct_capa…`
- `record_task_event`: `Report viewed, called, succeeded, failed or skipped capability status, or task stage. Usage and outcomes remain client-reported.`
- `resolve_daystruct_bundle`: `Read a saved, owned or public bundle with pinned source versions and current member availability. Returns a composition plan, not an execut…`
- `resolve_task_capabilities`: `Select relevant capabilities progressively, or request full delivery. Charges the published resolve price (/api/v1/pricing) to a key with r…`
- `search_daystruct_library`: `Search this account's saved or owned capabilities and bundles. Returns a small shortlist; saving does not acquire, execute or grant access…`
- `search_entities`: `Deprecated: this evidence tool is no longer refreshed and will be removed on or after 2026-12-31. For building, use discover_daystruct_capa…`
- `select_model`: `Deprecated: this evidence tool is no longer refreshed and will be removed on or after 2026-12-31. For building, use discover_daystruct_capa…`

## Changes

- 2026-10-15: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-15/e5ff8779bfb56c541392.json): `1 tool(s) added; 19 field(s) changed; signals: length_more_than_doubled`
- 2026-10-10: [count changed, tool added](../../deltas/2026-10-10/e5ff8779bfb56c541392.json): `1 tool(s) added`
- 2026-09-26: [description changed](../../deltas/2026-09-26/e5ff8779bfb56c541392.json): `10 field(s) changed; signals: length_more_than_doubled`
- 2026-09-25: [description changed, schema changed](../../deltas/2026-09-25/e5ff8779bfb56c541392.json): `4 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-09-24: [count changed, tool added](../../deltas/2026-09-24/e5ff8779bfb56c541392.json): `2 tool(s) added`
- 2026-09-23: [description changed](../../deltas/2026-09-23/e5ff8779bfb56c541392.json): `1 field(s) changed`
- 2026-09-21: [description changed, schema changed](../../deltas/2026-09-21/e5ff8779bfb56c541392.json): `33 field(s) changed; signals: length_more_than_doubled`
- 2026-09-14: [count changed, tool added](../../deltas/2026-09-14/e5ff8779bfb56c541392.json): `5 tool(s) added`
- 2026-09-12: [count changed, tool added](../../deltas/2026-09-12/e5ff8779bfb56c541392.json): `4 tool(s) added`
- 2026-09-11: [count changed, tool added](../../deltas/2026-09-11/e5ff8779bfb56c541392.json): `1 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.daystruct.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
