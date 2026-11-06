# deskcrew.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/deskcrew.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://deskcrew.ai/api/mcp` | 4 | [`205841ce112b`](ffca880fe8ae75a7fcd4.json) | 2026-08-20 |

## Tools at `https://deskcrew.ai/api/mcp`

- `create_purchase_challenge`: `Begin a purchase. Provide the setup spec (see get_catalog for the schema; businessName, contactEmail and agentPurpose are required). Return…`
- `get_catalog`: `Get the DeskCrew.ai agentic catalog: what is for sale (a managed AI phone agent for a business), the exact price and payment rails, the spe…`
- `get_order_status`: `Check an order you placed. Provide the orderId and orderKey returned by submit_payment. Returns the fulfilment status: paid, provisioning,…`
- `submit_payment`: `Complete a purchase. Provide the same spec plus paymentSignature: the base64 PAYMENT-SIGNATURE header you produced by signing one of the pa…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://deskcrew.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
