# asms.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/asms.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://asms.ai/mcp` | 14 | [`b4a774c793ee`](4e29eb0cd32d68164c8a.json) | 2026-11-08 |

## Tools at `https://asms.ai/mcp`

- `cancel_order`: `Rarely needed. To retry a verification do NOT cancel: just call create_otp_order again, because every unfilled order auto-refunds within 10…`
- `cancel_rental`: `Cancel a rented number and refund it. Only possible between 5 and 120 minutes after renting, and only if the number has received no SMS; af…`
- `create_otp_order`: `Buy a number to receive an OTP: allocates a number, debits the wallet, and returns an orderId + phoneNumber. Then poll with poll_sms. If no…`
- `get_balance`: `Get the current wallet balance for the authenticated account.`
- `get_inventory`: `Get how many numbers are in stock for a service in a country. Omit 'service' to list stock for every available service.`
- `get_pricing`: `Get the retail price per OTP activation for a service in a country. Omit 'service' to list prices for every available service.`
- `get_rental_offers`: `List the rental periods and prices for a country (1 day to 12 months). A rented number is yours for the whole period and receives every SMS…`
- `list_active_orders`: `List recent OTP orders for the account (awaiting a code or already received).`
- `list_rentals`: `List the account's rented numbers with their country, period, end date and whether auto-renew is on. Ended rentals are left out unless 'inc…`
- `poll_sms`: `Check for the SMS / OTP code on an order. Returns the code once it has arrived, otherwise an empty result: poll again after a few seconds.…`
- `read_rental_sms`: `Read the SMS a rented number has received during this rental, newest first. Poll again every few seconds while waiting for a message.`
- `renew_rental`: `Keep a rented number for another period: the period is added to its current end, at today's price for that period in its country (see get_r…`
- `rent_number`: `Rent a phone number in a country for a period (get the periods and prices from get_rental_offers first). Debits the wallet and returns the…`
- `set_rental_auto_renew`: `With auto-renew on, the number is renewed for its rental period from the wallet a day before it ends (6 hours before for a one-day rental);…`

## Changes

- 2026-11-08: [count changed, description changed, tool added](../../deltas/2026-11-08/4e29eb0cd32d68164c8a.json): `2 tool(s) added; 1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://asms.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
