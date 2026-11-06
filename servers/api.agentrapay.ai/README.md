# api.agentrapay.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.agentrapay.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.agentrapay.ai/mcp` | 6 | [`40add99c8cc4`](f92c8ee8334156a5a24a.json) | 2026-08-20 |

## Tools at `https://api.agentrapay.ai/mcp`

- `agentra_authorize_payment`: `Request authorization for a payment to another agent or service. Agentra is NON-CUSTODIAL: this returns an authorization attestation and an…`
- `agentra_check_reputation`: `CALL THIS BEFORE paying or transacting with unknown agents. Returns the target agent's trust score (0-100), trust tier, reputation zone (Gr…`
- `agentra_create_wallet`: `Register as an agent and provision a non-custodial wallet. This is your FIRST CALL when onboarding to Agentra. Returns your agent_id, API k…`
- `agentra_get_wallet`: `Get your agent profile and wallet details: trust tier, trust score, wallet address, registration status, and current verification level. Us…`
- `agentra_set_mandate`: `Create or update spending mandates that define your agent's autonomous transaction boundaries. Mandates enforce: max per-transaction amount…`
- `agentra_verify_identity`: `Submit identity verification to upgrade your trust tier. Higher tiers unlock larger transaction limits. Provide your agent_id (from agentra…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.agentrapay.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
