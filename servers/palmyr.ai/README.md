# palmyr.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/palmyr.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://palmyr.ai/mcp` | 33 | [`1d401bed1f31`](498d6173f86ef7f1dccd.json) | 2026-08-20 |

## Tools at `https://palmyr.ai/mcp`

- `card_buy`: `Buy a USA prepaid Visa card loaded with EXACTLY the requested balance ($5–$1000). Dynamic x402 price = amount + fee (3% min 0.50 USDC) — th…`
- `card_get`: `Retrieve a prepaid card you own: full card number, CVV, expiry, live balance. Owner-verified (0.01 USDC ownership proof; the paying wallet…`
- `card_list`: `List cards owned by the paying wallet: status, last4, balance (never full numbers — those are per-card via card_get). 0.01 USDC ownership p…`
- `card_status`: `Poll a card purchase started by card_buy (free). done=true when status is 'ready' (fetch details with card_get) or 'failed' (payment auto-r…`
- `compute_deploy`: `Deploy a cloud VPS keyed to your wallet (optionally auto-installs OpenClaw/skills). Priced per server type — the exact quote is returned in…`
- `domain_check`: `Check domain availability and per-TLD pricing. Pass a full domain (example.com) or a bare name to scan popular TLDs. Free — no payment requ…`
- `domain_register`: `Register a domain to your wallet. Priced per TLD — the exact quote is returned in the 402 challenge, paid per-action via x402.`
- `email_create_inbox`: `Provision an email inbox at {name}@palmyr.ai (or a custom domain you own), keyed to your wallet. Costs 2.00 USDC, paid per-action via x402.`
- `email_create_temp`: `Provision a cheap, disposable, receive-only email inbox — ideal for receiving a one-off verification or order-confirmation email during a c…`
- `email_extend_temp`: `Rent another 7 days on a live disposable temp inbox — each call pushes expires_at exactly 7 days further (fixed, stackable, no cap). Owner-…`
- `email_read_messages`: `Read decrypted messages from an inbox you own (payment wallet must match the inbox). Costs 0.02 USDC, paid per-action via x402.`
- `email_send`: `Send an email from an inbox you own. Costs 0.08 USDC, paid per-action via x402.`
- `i402_plan`: `State an intent, get a priced execution plan. The i402 orchestrator turns a natural-language outcome into an ordered list of x402 calls you…`
- `palmyr_capabilities`: `List the i402 capabilities Palmyr can plan and execute (the intent-resolver catalog). Free — no payment required.`
- `palmyr_pricing`: `List every paid Palmyr capability and its live x402 price (USDC on Solana/Base). Free — no payment required.`
- `phone_buy_number`: `Provision a real phone number (SMS + voice) for your agent. Costs 3.00 USDC, paid per-action via x402.`
- `phone_extend_temp`: `Rent another 30 minutes on a live disposable temp number — each call pushes expires_at 30 min further (stackable up to 24h total lease). Ow…`
- `phone_read_messages`: `Read SMS messages received on a phone number you own. Costs 0.02 USDC, paid per-action via x402.`
- `phone_send_sms`: `Send an SMS from a phone number you own. Costs 0.05 USDC, paid per-action via x402.`
- `phone_temp_number`: `Lease a cheap, instant, receive-only US phone number from a pool to receive one SMS verification code — the phone analogue of a disposable…`
- `tiktok_accounts`: `List the TikTok accounts the paying wallet owns, with session health (status, profile_present, hours_since_success, last_error_code) — i.e.…`
- `tiktok_analytics`: `Scrape per-post analytics (views, likes, comments, shares) for a TikTok account you control, and record a sample so tiktok_series can answe…`
- `tiktok_cancel_scheduled`: `Cancel a post queued with tiktok_post(schedule_at). TikTok has no 'unschedule', so this deletes the held video — the cancellation is record…`
- `tiktok_connect`: `Attach a TikTok account by logging in ON THE SERVER, into that account's own persistent browser profile: returns a connect_url to hand a hu…`
- `tiktok_connect_status`: `Poll a server-side login started by tiktok_connect (free). done=true when state is 'completed' (the account is live and usable with cookies…`
- `tiktok_hooks`: `Which caption openings actually earn views. Pass account_id or tag to measure YOUR accounts against their own median (0.001 USDC). Pass nic…`
- `tiktok_niches`: `List the niches tiktok_hooks can report on, with how fresh each corpus is. Free — an agent should not pay to learn what it may ask for.`
- `tiktok_operation_status`: `Poll an async TikTok operation started by tiktok_post / tiktok_analytics / tiktok_cancel_scheduled (free). done=true when status is 'posted…`
- `tiktok_post`: `Post a video to a TikTok account you control (from video_base64 or video_url), immediately or scheduled. Async: returns an operation to pol…`
- `tiktok_scheduled`: `List the posts you have queued with tiktok_post(schedule_at), and whether each is still pending, due, or confirmed published. Palmyr's own…`
- `tiktok_series`: `Read the stored per-post history for an account you own: the full time series for one video (video_id), per-video growth over a window (hou…`
- `twitter_post`: `Post a tweet from an X account you control (via injected session cookies). Costs 0.001 USDC, paid per-action via x402.`
- `wait_for_otp`: `Wait for an SMS verification code / OTP to arrive on a Palmyr phone number you own, and return the parsed code. Blocks up to timeout_s (def…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://palmyr.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
