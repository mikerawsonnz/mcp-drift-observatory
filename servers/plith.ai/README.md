# plith.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/plith.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://plith.ai/api/mcp` | 15 | [`550029851059`](cb4a0b1a1e1b535ab34e.json) | 2026-08-20 |

## Tools at `https://plith.ai/api/mcp`

- `burnrate_budget`: `Get today's tracked LLM spend, per-model breakdown, projection, and budget alerts. Free — no credits charged.`
- `burnrate_estimate`: `Before executing a multi-step agent plan, estimate the total LLM cost. Returns per-step breakdown and optimization suggestions. If the esti…`
- `burnrate_optimize`: `Get a cheaper equivalent plan by substituting models with lower-cost alternatives. Call after burnrate_estimate if the estimated cost excee…`
- `burnrate_track`: `Log the actual cost of an LLM call after execution. Call this after every LLM request to build calibration data that improves burnrate_esti…`
- `dedupq_check`: `Before executing any LLM task, check if an identical or semantically similar task has already been completed. Returns cached result on hit,…`
- `dedupq_complete`: `After executing a task, store the result so future identical or similar tasks return a cache hit via dedupq_check. Costs 2 credits.`
- `guardrail_check`: `Evaluate a proposed agent action against your governance policies. Returns allow or deny with the matched policy reason. Requires at least…`
- `guardrail_create_policy`: `Create a persistent governance policy that guardrail_check evaluates on every subsequent call. Define rules using and/or/not operators over…`
- `pitfalldb_query`: `Check for known failure patterns before executing a task type. Returns pitfalls with severity, fix suggestions, and confidence scores. Afte…`
- `pitfalldb_report`: `Report an agent failure. PII-scrubbed before storage. Linked to existing pitfalls if similar. Free — no credits charged.`
- `qualitygate_validate`: `After your agent generates output, validate it against your rules before shipping. Runs deterministic checks (regex, JSON schema, syntax) p…`
- `rigor_execute`: `Execute a structured workflow end-to-end. Call rigor_plan first (free) to preview the step sequence and cost estimate before committing cre…`
- `rigor_plan`: `Before executing a complex task, get a structured workflow plan with per-step cost estimates. Classifies your task, selects the optimal fra…`
- `rigor_status`: `Check the status of a running or completed Rigor workflow. Returns progress, step results, and the full deliverable when complete. Use afte…`
- `rigor_workflows`: `List all Rigor workflows for your organization with filtering and pagination. Returns status, progress, capacity usage, and available actio…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://plith.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
