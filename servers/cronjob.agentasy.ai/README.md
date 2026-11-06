# cronjob.agentasy.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/cronjob.agentasy.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://cronjob.agentasy.ai/mcp` | 15 | [`e549a18006de`](4032322e3d32d36b8436.json) | 2026-11-04 |

## Tools at `https://cronjob.agentasy.ai/mcp`

- `claim_credentials`: `Step 3. Poll verification state with the setup_token. The first call after the webhook is verified returns hmac_secret (signs triggers) and…`
- `create_job`: `Step 1. Register your webhook and schedule (no account, no API key). Returns job_id and a one-time setup_token, and POSTs a url_verificatio…`
- `delete_job`: `Stop the job forever and revoke all its credentials. Cannot be undone. (REST: DELETE /v1/jobs/{id})`
- `get_deliveries`: `Trigger log, newest first: scheduled_at, first attempt time, delay, attempts, status and last response code of each run. since/until (ISO 8…`
- `get_job`: `Settings, status, next_run_at, run_count and credential prefixes of one job (webhook path masked). (REST: GET /v1/jobs/{id})`
- `get_run`: `One run and each delivery attempt: sent_at, response status, duration, error and next retry. (REST: GET /v1/jobs/{id}/runs/{run_id})`
- `get_stats`: `On-time rate, p50/p95 first-attempt delay and success rate over a window (default 24h). (REST: GET /v1/jobs/{id}/stats)`
- `list_jobs`: `Status of every job you hold a management token for. There are no accounts, so pass each {job_id, management_token} pair (up to 20); a pair…`
- `pause_job`: `Stop triggering (idempotent). Schedule points while paused are not made up later. (REST: POST /v1/jobs/{id}/pause)`
- `resume_job`: `Resume a paused or disabled job from its next schedule point; resets consecutive_failures. (REST: POST /v1/jobs/{id}/resume)`
- `retry_challenge`: `Re-send a fresh url_verification challenge to your webhook (at most 5 re-sends (6 challenges in total), at least 60 s apart). The previous…`
- `rotate_secret`: `New hmac_secret (SHOWN ONCE, store it now). Until previous.expires_at (grace_sec, default 24 h) triggers carry two v1= signatures, new firs…`
- `rotate_token`: `New management_token (SHOWN ONCE, store it now). The old one stops working after grace_sec (default 0 = immediately). (REST: POST /v1/jobs/…`
- `update_job`: `Change a job in place: signature_in_body (true = triggers also carry cronjob_signature in the JSON body, for platforms that drop the X-Cron…`
- `verify_challenge`: `Step 2 (callback mode). Send back the challenge value your webhook received. On success the result holds hmac_secret and management_token —…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://cronjob.agentasy.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
