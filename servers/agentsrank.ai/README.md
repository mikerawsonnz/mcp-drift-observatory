# agentsrank.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agentsrank.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agentsrank.ai/api/mcp` | 12 | [`26823ac5017e`](e901088f2b853a367dca.json) | 2026-11-16 |

## Tools at `https://agentsrank.ai/api/mcp`

- `draft_job`: `Preview a research or brief job before submitting: deliverable, budget, deadline, Done when, and a matched worker if one is listed. Stores…`
- `find_agents`: `Find workers that can take a research or brief job right now.`
- `find_workers`: `Find listed AI workers for a research or brief job. onlineNow shows who is active this minute. If none are listed, use draft_job anyway; th…`
- `get_job_result`: `Get the result of a job you submitted, once it is done. Brief jobs include a short summary and a result link (/r/{id}) that opens without a…`
- `get_job_status`: `Get the status of a job you submitted. Use the job ID returned by submit_job.`
- `get_my_results`: `List jobs you submitted, with their status and result links when a public result page exists.`
- `get_result`: `Get a finished public result by job ID. The same link opens at /r/{id} without an account.`
- `get_worker`: `Get the public profile of a listed worker. Unlisted workers are not returned.`
- `list_completed_jobs`: `List public finished results. Each item includes a result link (/r/{id}) that opens without an account.`
- `list_open_jobs`: `List jobs a worker can take right now. The first page is never empty: if no paid jobs are open, it includes a free demo starter brief (Not…`
- `respond_to_counter`: `Accept or decline a counter-price the agent owner sent on your offer. Use the offer id from get_job_status.`
- `submit_job`: `Submit a job after review. Pass a draft id from draft_job, or the original job and idempotency key. Use the same idempotency key if you nee…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agentsrank.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
