# app-emailwarmup.bobwork.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app-emailwarmup.bobwork.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app-emailwarmup.bobwork.ai/mcp` | 46 | [`8815102e9c2f`](05c4b5d497c7d086d782.json) | 2026-11-04 |

## Tools at `https://app-emailwarmup.bobwork.ai/mcp`

- `add_contacts`: `Add up to 1,000 contacts to a campaign. Each needs email; other fields (first_name, company…) fill the placeholders. Duplicates and unsubsc…`
- `add_dns_record`: `Add a DNS record to a domain you bought here. name = subdomain ('' for the domain itself). Types A, AAAA, CNAME, ALIAS, MX, TXT, CAA, SRV.`
- `add_hosted_mailboxes`: `Add mailboxes to a domain you bought here ($3 per mailbox per month). Returns a Stripe checkout link.`
- `buy_domains`: `Buy domains with up to 3 mailboxes each. Returns a Stripe checkout link for the person to pay; setup starts once paid. Needs accept_sending…`
- `check_dkim`: `Find a domain's DKIM key: tries the selector you give, selectors seen in real mail, then 45 common ones.`
- `check_dmarc`: `Look up a domain's DMARC record and policy.`
- `check_spf`: `Look up a domain's SPF record.`
- `connect_imap_mailbox`: `Connect any mailbox with IMAP + SMTP. The login is tested before it is saved. Use an app password when two-factor sign-in is on. Give a pre…`
- `connect_zoho_mailbox`: `Connect a Zoho Mail mailbox through the Zoho API (works on Zoho's free plan). Needs a Self Client id, secret and a generated code from api-…`
- `create_billing_checkout`: `Get a Stripe Checkout url for extra mailboxes beyond the free limit (monthly, or yearly = 10 months' price for 12). The USER opens it and p…`
- `create_campaign`: `Create a draft Outbound campaign (nothing is sent). Emails can use {first_name}, {company} and any contact field. Any connected mailbox can…`
- `create_credits_checkout`: `Get a Stripe Checkout url to top up prepaid credits for Outbound sending and AI drafts (one-off $5, $10, $25 or $100; credits never expire)…`
- `create_workspace`: `Create a client workspace, e.g. the client's company name (max 100 per account).`
- `delete_dns_record`: `Delete a DNS record by id (from list_dns_records). Deleting MX, SPF, DKIM or DMARC stops the mailboxes working.`
- `delete_workspace`: `Delete a client workspace. Its mailboxes are NOT deleted: they move back to My mailboxes and keep warming. The client's report link stops w…`
- `domain_health`: `SPF, DKIM selector, DMARC policy and MX for every domain you have connected.`
- `get_account`: `Your account: email, credit balance, free mailbox allowance (10, or 20 for accounts created before 27 October 2026, plus referral bonus), p…`
- `get_billing_status`: `Payment status after you gave the user a checkout link: credit balance, whether the extra-mailbox subscription is active, mailboxes vs the…`
- `get_campaign`: `One campaign: its emails, mailboxes, stats and time left.`
- `get_credits`: `Prepaid credit balance, prices and recent charges (Outbound emails, AI drafts).`
- `get_mailbox`: `One mailbox's warm-up status and health.`
- `get_workspace_report`: `The public read-only report link for one client workspace (mailbox health, spam rate, SPF/DKIM/DMARC). The client opens it without a login;…`
- `google_connect_link`: `Get a link the user opens to connect Gmail / Google Workspace with Google sign-in (one click, any device). The mailbox appears in list_mail…`
- `hosted_mailbox_login`: `Password, IMAP and SMTP settings for one of your hosted mailboxes.`
- `list_bought_domains`: `Domains bought in the domain shop, their hosted mailboxes, renewal date and price, plus IMAP/SMTP settings.`
- `list_campaign_contacts`: `Contacts in a campaign and where each is in the sequence (first 200).`
- `list_campaigns`: `Your Outbound campaigns with status and stats.`
- `list_dns_records`: `DNS records on a domain you bought here.`
- `list_mailboxes`: `Every connected mailbox with warm-up day, status, 7-day spam rate, today's and last 7 days' numbers, and whether it is ready for outbound.`
- `list_providers`: `IMAP/SMTP presets (Gmail app password, Yahoo, iCloud, Zoho, Lark, SES, SendGrid, Mailgun…) with hosts and ports, plus the Google and Zoho A…`
- `list_workspaces`: `Client workspaces (agencies): each client's mailboxes are kept separate under one login and one bill. Returns id, name and mailbox count. E…`
- `mailbox_activity`: `The last 100 warm-up events for a mailbox (sent, received, replied, rescued from spam, errors).`
- `move_mailbox_to_workspace`: `Put a mailbox in a client workspace. Leave workspace_id out (or empty) to move it back to My mailboxes.`
- `pause_campaign`: `Pause a running campaign.`
- `pause_mailbox`: `Pause warm-up for a mailbox.`
- `remove_mailbox`: `Remove a mailbox and delete its stored login. Irreversible: ask the user first, then pass confirm=true.`
- `rename_workspace`: `Rename a client workspace.`
- `resume_mailbox`: `Resume warm-up for a mailbox.`
- `search_domains`: `Find available lookalike domains for cold email, with first-term and renewal prices.`
- `set_pool_mode`: `Shared network (default: warm with every mailbox on the service) or private pool (only your own mailboxes write to each other; needs 2+).`
- `set_warm_style`: `Teach warm-up mail how you write: paste up to 4,000 characters of your own sent emails (tone, length, sign-offs). Empty clears it. Used whe…`
- `start_campaign`: `Start or resume a campaign. This SENDS real email and uses credits. Confirm with the user first. accept_sending_rules=true means the user a…`
- `test_mailbox`: `Sign in to the mailbox now and report whether the stored login still works.`
- `update_campaign`: `Edit a paused or draft campaign. Fields you leave out keep their value.`
- `update_mailbox`: `Change a mailbox's display name, daily warm-up cap (1-100, null = default), time zone (IANA, e.g. Europe/London) or the signature added to…`
- `warmup_stats`: `Totals across your mailboxes: today and last 7 days (sent, received, rescued, replied), active and ready counts.`

## Changes

- 2026-11-04: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-04/05c4b5d497c7d086d782.json): `1 tool(s) added; 3 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app-emailwarmup.bobwork.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
