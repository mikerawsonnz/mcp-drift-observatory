# mcp.agenticterminal.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.agenticterminal.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.agenticterminal.ai/mcp` | 6 | [`5debd2ae2310`](977dc2cf686645e4439c.json) | 2026-08-20 |

## Tools at `https://mcp.agenticterminal.ai/mcp`

- `get_merchant`: `Get the full record for one merchant including all rails, payment endpoints, and OP attestation. Tier 2+ requires an AT credential.`
- `list_categories`: `List the category taxonomy with merchant counts.`
- `list_rails`: `List supported payment rails and their current merchant counts.`
- `search_merchants`: `Search OP-verified merchants by rail, chain, category, agent-callable tier, trust tier, and free text. Ranked by trust tier then verificati…`
- `verify_payment_endpoint`: `Run a live check against a merchant's declared payment endpoint for a rail. Returns health, detail, and rail-specific evidence.`
- `whoami`: `Report the resolved credential state and rate limits for the calling agent.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.agenticterminal.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
