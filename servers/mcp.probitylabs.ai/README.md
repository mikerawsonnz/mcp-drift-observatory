# mcp.probitylabs.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.probitylabs.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.probitylabs.ai/mcp` | 6 | [`5e459ac862d7`](0db8ca6eb99ec8092016.json) | 2026-08-20 |

## Tools at `https://mcp.probitylabs.ai/mcp`

- `compare_screening_runs`: `Compare two completed screens by their screeningId and see what changed. Costs zero credits. Two runs of the same address show why the repu…`
- `get_address_screening_history`: `Retrieve the authenticated user's prior screening runs for a specific Ethereum address, each with the same detail as screen_address: reputa…`
- `get_credit_balance`: `Returns the authenticated user's current credit balance as a whole number of credits. One credit screens one address: screen_address costs…`
- `get_screening_history`: `Returns the authenticated user's most recent screening runs across all addresses, newest first, each with the same detail as screen_address…`
- `get_screening_narrative`: `Retrieve the enhanced Probity review for a completed screen by its screeningId. Costs zero credits. Returns the narrative and the key conce…`
- `screen_address`: `Screen an Ethereum address or '.eth' ENS name for on-chain reputation risk. Costs 1 credit. Returns a signed reputation score (-100 to +100…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.probitylabs.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
