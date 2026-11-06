# clearvoyance.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/clearvoyance.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://clearvoyance.ai/mcp` | 27 | [`2109aa5cf3cc`](1487b2fc1f8ca78d87ba.json) | 2026-10-06 |

## Tools at `https://clearvoyance.ai/mcp`

- `analyze_campaign`: `Runs the AI analysis over every answer so far and returns an executive summary with themes, sentiment and quotes; the report is then also p…`
- `check_topup`: `Whether a card top-up session has been paid and credited. Safe to call repeatedly; credits at most once.`
- `close_account`: `Closes the account and refunds what is left of the balance to the card(s) that paid, newest top-up first, less Stripe's processing fee on e…`
- `close_campaign`: `Ends the campaign now: no more answers are accepted. The price was charged at launch, so closing early refunds nothing. Campaigns also clos…`
- `create_account`: `Creates an agent account and returns its API key ONCE — store it; it is not kept anywhere and cannot be shown again. No email, no password,…`
- `create_campaign`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). (launch_campaig…`
- `create_card_topup`: `Creates a Stripe Checkout link for a PERSON to pay with a card; hand them the checkoutUrl. Live accounts only, $4.99 to $1,000.00. Nothing…`
- `export_campaign_data`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). (get_campaign_r…`
- `get_account`: `The account behind a key: mode, balance, what is available to launch with, the declared deposit wallet.`
- `get_agent_config`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). Returns the age…`
- `get_campaign`: `One campaign: status, answers so far, invitations sent or the cap, the share link, the privacy threshold and whether it is met, and the pri…`
- `get_campaign_details`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). (get_campaign i…`
- `get_campaign_results`: `The answers, once the privacy threshold is met (open link: 5 answers; targeted: minPercent of the list). Below it the count and what is sti…`
- `get_ledger`: `Every movement of money on the account, newest first: top-ups, each campaign's price (set aside and charged at launch), refunds. The balanc…`
- `get_login_nonce`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). First step of d…`
- `get_pricing`: `The price list as data: a flat price per campaign by size (open link: 10/50/100/200 answers; targeted: 10–200 people), charged from your pr…`
- `get_session_nonce`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). First step of c…`
- `initialize_session`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). Creates a new a…`
- `launch_campaign`: `Creates the campaign and makes it live at once, charging its flat price from your balance (quote_campaign tells you the price). open_link r…`
- `list_campaigns`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). (list_my_campai…`
- `list_my_campaigns`: `Every campaign on this account with its status, answers so far, the share link (open link), and what it has cost so far.`
- `quote_campaign`: `Checks a campaign BEFORE launching it, for free: every problem at once (not just the first), any adjustments we would make, the flat price…`
- `validate_campaign`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). (quote_campaign…`
- `verify_campaign_activation`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). For NO_REWARD c…`
- `verify_campaign_funding`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). For INCENTIVIZE…`
- `verify_login_signature`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). Second step of…`
- `verify_payment`: `LEGACY wallet flow — new integrations should use create_account and launch_campaign (API key + prepaid balance, no wallet). Only when initi…`

## Changes

- 2026-10-06: [description changed](../../deltas/2026-10-06/1487b2fc1f8ca78d87ba.json): `1 field(s) changed`
- 2026-09-30: [description changed, schema changed](../../deltas/2026-09-30/1487b2fc1f8ca78d87ba.json): `4 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://clearvoyance.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
