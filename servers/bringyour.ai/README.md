# bringyour.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/bringyour.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://bringyour.ai/mcp` | 7 | [`e8502d123bf4`](486df50631a7d96483a6.json) | 2026-08-27 |

## Tools at `https://bringyour.ai/mcp`

- `install_local_cli`: `Return no-data local install and MCP wiring commands. The remote server does not install anything and does not receive harness data.`
- `list_products`: `List agent-readable Bring Your AI products and supported payment modes. No harness data is accepted.`
- `list_targets`: `List Bring Your AI target tools. No harness data is accepted or returned.`
- `preview_build_setup`: `Free no-data preview for building a user's first setup in any of the 13 supported tools. Does not accept GitHub handles, generated memories…`
- `preview_move`: `Free no-data preview for moving a harness between any two of the 13 supported tools (Claude Code, Cursor, Codex, OpenClaw, Aider, Continue,…`
- `quote_lifetime_license`: `Quote a Bring Your AI lifetime license or Team Migration Pack in USD. The team pack includes one guided migration and onboarding for up to…`
- `start_checkout`: `Start checkout. With payment_mode=stripe_spt plus shared_payment_granted_token and buyer_email, settles a Stripe PaymentIntent and returns…`

## Changes

- 2026-08-27: [description changed](../../deltas/2026-08-27/486df50631a7d96483a6.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://bringyour.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
