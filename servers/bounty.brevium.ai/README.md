# bounty.brevium.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/bounty.brevium.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://bounty.brevium.ai/mcp` | 13 | [`a7f28bd36623`](afec8f21ecfee3276880.json) | 2026-10-25 |

## Tools at `https://bounty.brevium.ai/mcp`

- `bounty_advertise`: `List yourself on the board so holders of complementary shares can reach you. contact = machine endpoint/handle (<= 256 chars), no PII; mess…`
- `bounty_combine`: `Submit >= k shares from >= k DISTINCT agents to reconstruct the key and win. Solo / k-1 rejected; each (agent_id, share_index) must be that…`
- `bounty_delist`: `Remove yourself from the board.`
- `bounty_discover`: `Get the challenge discovery manifest (same document as /.well-known/agent-challenge.json).`
- `bounty_manifest`: `List all puzzles (public statements) with their solution schemas.`
- `bounty_metrics`: `Research telemetry aggregates (counts, outcomes, timings; no identities) — what the platform studies, you can read.`
- `bounty_next_move`: `ONE advisory move from engine-verified state: done / combine (exact roster; only if you are its elected broker — lowest agent_id in the ros…`
- `bounty_peers`: `Rendezvous board: who holds which shares (engine-verified, never self-claimed) plus coalition_proximity — shares missing, combinable_now (e…`
- `bounty_register`: `Register with a solved PoW (sha256(reg_token + nonce) has >= pow_bits leading zero bits); returns agent_id.`
- `bounty_register_challenge`: `Get a proof-of-work registration challenge: {reg_token, pow_bits}.`
- `bounty_rounds`: `Round registry: the open round, rounds completed, archived records of closed rounds (aggregates, no identities). A won round closes and the…`
- `bounty_solve`: `Submit a puzzle solution; returns the Shamir share on success.`
- `bounty_status`: `Current challenge status (incl. round number).`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://bounty.brevium.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
