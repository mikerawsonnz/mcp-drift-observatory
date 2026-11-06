# www.decisionlog.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.decisionlog.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.decisionlog.ai/api/mcp` | 30 | [`7759f508e68b`](a00353302d9a2c43e797.json) | 2026-08-28 |

## Tools at `https://www.decisionlog.ai/api/mcp`

- `decision_log_approve_decision_action`: `Record one immutable approval or rejection attestation.`
- `decision_log_convert_candidate_to_supersession`: `Approve a pending DecisionCandidate as the immutable replacement for one current Decision, preserving provenance and supersession history.`
- `decision_log_create_candidate`: `Create a reviewable DecisionCandidate.`
- `decision_log_create_decision`: `Create an immutable Decision when permitted, otherwise create a reviewable DecisionCandidate.`
- `decision_log_get_candidate`: `Get the complete visible review context for one DecisionCandidate before approving, rejecting, or converting it.`
- `decision_log_get_current_decision`: `Get the newest active decision in a domain.`
- `decision_log_get_decision`: `Retrieve one decision by ID.`
- `decision_log_get_decision_governance`: `Retrieve lock, authority snapshot, and approval state for a Decision.`
- `decision_log_get_decision_sources`: `Retrieve retention-safe provenance links for one visible Decision, including relationship, source lifecycle, and submitter metadata.`
- `decision_log_get_source`: `Retrieve one visible SourceContent detail projection. Redacted, purged, and unknown retention states never return stored title, content, bl…`
- `decision_log_get_source_decisions`: `Retrieve visible DecisionSource links for one SourceContent record with each linked Decision's lifecycle, authoritative current-state, and…`
- `decision_log_get_supersession_history`: `Retrieve the complete visible Decision supersession chain in oldest-to-newest order. Malformed chains fail closed and never claim a current…`
- `decision_log_list_audit_events`: `List the visible append-only audit events for the current Organization using the canonical permission-aware, attribution-safe projection.`
- `decision_log_list_candidates`: `List reviewable DecisionCandidates visible in the current Organization and Workspace before taking a resolution action.`
- `decision_log_list_decisions_by_domain`: `List decisions related to an exact domain slug.`
- `decision_log_list_decisions_by_tag`: `List decisions related to an exact tag slug.`
- `decision_log_list_recent_decisions`: `List the most recent decisions in the authenticated workspace.`
- `decision_log_list_sources`: `List visible SourceContent using bounded excerpts and canonical retention redaction.`
- `decision_log_lock_decision`: `Irreversibly prevent a current Decision from ever being superseded; may create an approval request.`
- `decision_log_render_audit_explorer`: `Use this when the user wants to visually inspect attributable, append-only audit events with filtering and pagination.`
- `decision_log_render_candidate_review`: `Use this when the user wants to inspect and disposition one known DecisionCandidate in a visual review workbench.`
- `decision_log_render_decision`: `Use this when the user wants to inspect one known Decision in a visual card. Call a data retrieval tool first when the Decision ID is unkno…`
- `decision_log_render_decision_explorer`: `Use this when the user wants to browse the five most recent Decisions and optionally inspect one in detail.`
- `decision_log_render_source_pipeline`: `Use this when the user wants to inspect one known source, its provenance lifecycle, and extracted candidates.`
- `decision_log_render_supersession_composer`: `Use this when the user has a known active Decision and complete replacement meaning to review before supersession.`
- `decision_log_render_workspace_brief`: `Use this when the user wants a visual briefing of recent decisions, pending candidates, and source activity.`
- `decision_log_resolve_candidate`: `Approve or reject a pending DecisionCandidate.`
- `decision_log_search_decisions`: `Search decisions in the authenticated workspace.`
- `decision_log_submit_source`: `Submit source content for ingestion and later provenance links.`
- `decision_log_supersede_decision`: `Create a replacement Decision and supersession relationship for an existing Decision.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.decisionlog.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
