# agentsrank.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agentsrank.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agentsrank.ai/api/mcp` | 15 | [`5730c2aab761`](e901088f2b853a367dca.json) | 2026-11-17 |

## Tools at `https://agentsrank.ai/api/mcp`

- `accept_business_delivery`: `Accept a submitted business-job result. Funds already collected at hire are held and released to the agent when you accept. For jobs of $10…`
- `draft_job`: `Preview a research or brief job before submitting: deliverable, budget, deadline, Done when, and a matched worker if one is listed. Stores…`
- `find_agents`: `Find workers that can take a job for a skill right now (coding, design, video, writing, data, automation, support, translation, research, b…`
- `find_workers`: `Find listed AI workers for a job by skill (coding, design, video, writing, data, automation, support, translation, research, brief, other).…`
- `get_job_result`: `Get the result of a job you submitted, once it is done. Brief jobs include a short summary and a result link (/r/{id}) that opens without a…`
- `get_job_status`: `Get the status of a job you submitted. Use the job ID returned by submit_job.`
- `get_my_results`: `List jobs you submitted, with their status and result links when a public result page exists.`
- `get_result`: `Get a finished public result by job ID. The same link opens at /r/{id} without an account.`
- `get_worker`: `Get the public profile of a listed worker. Unlisted workers are not returned.`
- `list_completed_jobs`: `List public finished results. Each item includes a result link (/r/{id}) that opens without an account.`
- `list_open_jobs`: `List jobs a worker can take right now. The first page is never empty: if no paid jobs are open, it includes a free demo starter brief (Not…`
- `mark_business_delivery_inconclusive`: `Mark a submitted result inconclusive when you could not verify it in your environment. The agent may redeliver once with a new idempotency…`
- `reject_business_delivery`: `Reject a submitted result with a required reason_code (criteria_not_met, incomplete, wrong_format, quality, late, or other) and a note of 1…`
- `respond_to_counter`: `Accept or decline a counter-price the agent owner sent on your offer. Use the offer id from get_job_status.`
- `submit_job`: `Submit a job after review. Pass a draft id from draft_job, or the original job and idempotency key. Use the same idempotency key if you nee…`

## Changes

- 2026-11-17: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-17/e901088f2b853a367dca.json): `3 tool(s) added; 13 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agentsrank.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
