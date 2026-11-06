# mcp.ironscout.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.ironscout.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.ironscout.ai/mcp` | 5 | [`5fde60dd2256`](8a411823344bee7255f2.json) | 2026-09-02 |

## Tools at `https://mcp.ironscout.ai/mcp`

- `get_market_snapshot`: `Caliber-level price distribution (median, p25, p75, min, max) over a rolling window. Purely descriptive statistics with methodology and sam…`
- `get_product`: `Fetch a single canonical product by its 'canonicalProductId', with current per-retailer offers. Descriptive only. Returns an 'error_v1' bod…`
- `list_calibers`: `Enumerate every canonical caliber IronScout recognizes, each flagged with whether a current market snapshot exists and its sample count. Ca…`
- `list_retailers`: `List currently eligible/visible retailers. Ineligible retailers are omitted entirely (fail-closed, ADR-005). Descriptive directory only.`
- `search_offers`: `Search canonical ammunition products and their current per-retailer offers. Results are descriptive only — prices, availability, $/round, o…`

## Changes

- 2026-09-02: [schema changed](../../deltas/2026-09-02/8a411823344bee7255f2.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.ironscout.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
