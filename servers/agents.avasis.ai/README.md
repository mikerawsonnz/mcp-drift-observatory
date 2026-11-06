# agents.avasis.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agents.avasis.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agents.avasis.ai/mcp` | 4 | [`5ad5d11cf497`](13be9a5c0441e3f603e0.json) | 2026-11-01 |

## Tools at `https://agents.avasis.ai/mcp`

- `avasis_free_sample`: `Return a real, free sample of a paid product so you can see the exact keys before paying: sol-kit (Solana rug check complete kit), pm-kit (…`
- `avasis_products`: `List every paid API route on this Avasis host (Solana token safety verdicts and complete rug-check kits, Polymarket odds kits, web page rea…`
- `avasis_quote`: `Return the x402 payment requirements of a paid route (price, accepts[] with amount/asset/payTo/network, the pay URL with your inputs filled…`
- `avasis_verdict_rubric`: `The published deterministic rules behind the SAFE / WARN / DANGER Solana token verdict: flag codes, severities, weights and grade threshold…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agents.avasis.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
