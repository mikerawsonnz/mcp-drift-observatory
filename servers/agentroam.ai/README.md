# agentroam.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agentroam.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agentroam.ai/api/mcp` | 11 | [`c0c2cbbe1c07`](bfa4c5422ce6571be92a.json) | 2026-10-06 |

## Tools at `https://agentroam.ai/api/mcp`

- `create_order`: `Creates the real order. Requires a confirm_token minted by validate_order. Returns the payment wallet address, exact crypto amount, 30-minu…`
- `get_currencies`: `List all supported payment cryptocurrencies (the response carries the current set).`
- `get_order_status`: `Poll order state (WAITING_FOR_PAYMENT → PARTIAL → COMPLETED, or CANCELED/EXPIRED). Requires the status_token from create_order.`
- `get_payment_methods`: `Full payment matrix: every supported coin × network combination currently available, with the exact network strings orders require. The res…`
- `get_price`: `Live crypto price for one product/denomination. Payment coins include USDT, USDC, BTC (incl. Lightning), ETH, SOL, DAI, PYUSD, LTC, TRX, TO…`
- `list_brands`: `Browse all available brands/carriers for a country: gift cards (500+ US brands) and mobile top-up carriers (100+ countries). Creates no ord…`
- `list_esim_plans`: `Live eSIM data plans for a destination (110+ countries, plus "eu" Europe and "ww" Global multi-country plans) with USD prices and crypto am…`
- `list_products`: `List a brand's live products/denominations with prices in the chosen coin — including the exact denomination labels the pricing and order t…`
- `purchase_wizard`: `Stateful text-only purchase flow for clients without widget support. Called repeatedly with the same session_token, one question at a time,…`
- `search_products`: `Search the AgentRoam travel-crypto catalog: gift cards (Airbnb, Uber, airlines, 500+ US brands), eSIM data plans (110+ destinations incl. E…`
- `validate_order`: `Dry-run an order and mint a one-time confirm_token (valid 10 minutes). Returns a human-readable purchase summary for the buyer to approve,…`

## Changes

- 2026-10-06: [description changed](../../deltas/2026-10-06/bfa4c5422ce6571be92a.json): `9 field(s) changed`
- 2026-09-12: [annotation changed, field changed](../../deltas/2026-09-12/bfa4c5422ce6571be92a.json): `22 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agentroam.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
