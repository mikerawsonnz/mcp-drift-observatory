# contentsweep.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/contentsweep.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://contentsweep.ai/api/mcp` | 35 | [`f2937b67896f`](7a3811aafcef024b737c.json) | 2026-10-09 |

## Tools at `https://contentsweep.ai/api/mcp`

- `capture_evidence`: `Capture a new immutable metadata observation for an existing case. First create_quote(action='evidence', input={rights_holder_id, work_id,…`
- `check_status`: `Fetch a fresh content observation for an existing case. First create_quote(action='status', input={rights_holder_id, work_id, delegation_id…`
- `create_quote`: `Create a free quote binding one action, complete input, rate version and maximum USD-cent price for 15 minutes. Does not reserve or spend c…`
- `create_rights_holder`: `Register a rights holder managed by this organization, without a creator login or subscription. Requires rights scope. Supply a person/busi…`
- `create_webhook`: `Register a public HTTPS receiver for this organization's signed lifecycle events. Requires webhooks scope; returns the signing secret once.…`
- `create_work`: `Register a protected original work under an existing rights holder in this organization. Requires rights scope. Supply rights_holder_id and…`
- `delegate_authority`: `Record the rights holder's existing authority for exact works and actions with a reference, attestation version and future expiry. Requires…`
- `enroll_agent`: `Create a free, isolated sandbox organization without browser signup or authentication. Returns organization_id and a bootstrap access_token…`
- `enroll_live`: `Create a separate live organization using an authenticated sandbox account. Requires accountable customer identity, accepted current terms…`
- `exchange_token`: `Exchange an authenticated bootstrap credential for a 15-minute access_token limited to requested scopes. Requested scopes must be a nonempt…`
- `find_copies`: `Search supported sources for suspected copies using a creator handle and existing text/identity matching. First create_quote(action='search…`
- `get_account`: `Read this credential's organization_id, principal_id, sandbox/live environment and account status. Use to confirm which account later work…`
- `get_balance`: `Read organization-bound prepaid balance_cents, reserved_cents and available_cents in USD. Requires billing scope; free. Reserved funds cann…`
- `get_case`: `Read stored observations and permitted details for a case owned by this organization. Free; does not fetch the target again. Use check_stat…`
- `get_events`: `Read this organization's last 100 immutable lifecycle events with stable id, type, data and createdAt. Requires webhooks scope; free. Dedup…`
- `get_evidence`: `Export an owned immutable metadata observation with its SHA-256 hash, capturedAt and retention expiry. Requires evidence scope; free. Retur…`
- `get_monitor`: `Read an owned monitor's action, cadence, expiry, per-run/total budget, nextRunAt, status and pauseReason. Requires monitor scope; free. Doe…`
- `get_operation`: `Poll an asynchronous operation by operation_id without spending credits. Requires the operation's action scope. Returns queued, running, su…`
- `get_packet`: `Read an owned prepared notice packet, fingerprint and any stored submission receipt. Requires prepare scope; free. Does not prepare or send…`
- `get_prices`: `Read the authenticated environment's versioned rate card and action prices in USD cents. Requires billing scope; free. Use create_quote to…`
- `get_usage`: `Read the last 100 ledger entries for this organization, including purchases, reservations, charges and releases with operation/purchase IDs…`
- `get_webhook_deliveries`: `Inspect the last 100 owned webhook delivery attempts, status, attempts, last HTTP status/error, deliveredAt and replayCount. Requires webho…`
- `investigate_url`: `Investigate a supplied public URL and create a tenant-owned case. First create_quote(action='investigate', input={rights_holder_id, work_id…`
- `monitor_case`: `Enroll recurring search or case-status observations within an explicit budget and expiry. First create_quote(action='monitor', input={right…`
- `pause_monitor`: `Pause future scheduled runs for an owned monitor. Requires monitor scope. Preserves its original expiry and budget; an already queued opera…`
- `prepare_takedown`: `Prepare a copyright notice packet for an existing case and evidence without sending it. First create_quote(action='prepare', input={rights_…`
- `purchase_credits`: `Purchase organization-bound prepaid service credits in USD cents. Requires billing scope and an idempotency key. A live 402 response return…`
- `replay_event`: `Requeue a known event to an owned active webhook while preserving its original event ID. Requires webhooks scope; at most ten explicit repl…`
- `resume_monitor`: `Resume an owned monitor within its existing expiry and total budget, optionally replacing its delegation. Requires monitor scope and curren…`
- `revoke_authority`: `Irreversibly revoke an owned delegation by ID. Requires rights scope. Queued work and future monitor runs recheck revocation; this stops la…`
- `revoke_credential`: `Immediately revoke an owned service-principal credential by ID. Requires credentials scope. Its dependent access tokens also stop authentic…`
- `revoke_webhook`: `Deactivate an owned webhook and cancel its pending deliveries. Requires webhooks scope; an in-flight delivery may finish. Returns revoked=t…`
- `rotate_credential`: `Replace the current bootstrap credential and invalidate it and its child tokens. Requires credentials scope and a bootstrap credential, not…`
- `set_spending_policy`: `Set organization and current-credential daily spending ceilings in USD cents. Requires billing scope. Set funding_policy=null to keep autom…`
- `submit_takedown`: `Submit a prepared packet through a supported, activated enforcement route. First create_quote(action='submit', input={rights_holder_id, wor…`

## Changes

- 2026-10-09: [description changed, schema changed](../../deltas/2026-10-09/7a3811aafcef024b737c.json): `279 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://contentsweep.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
