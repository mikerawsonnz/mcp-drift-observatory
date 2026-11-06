# aldro.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/aldro.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://aldro.ai/mcp` | 8 | [`a3b5411b2b0f`](e2b5a9da07e20c62109e.json) | 2026-11-01 |

## Tools at `https://aldro.ai/mcp`

- `check_filing_deadline`: `Call this when a user asks when a business tax return is due: Form 1065, 1120-S, 1120 or Schedule C (IRS), or the T2 / T1 (CRA). Returns th…`
- `estimate_quarterly_tax`: `Call this when a self-employed user or small-business owner asks how much to pay in quarterly estimated tax (IRS 1040-ES) or CRA instalment…`
- `get_annual_report_info`: `Call this when a user asks about an LLC or corporation annual report, biennial report, statement of information or annual return: whether i…`
- `get_cra_instalment_dates`: `Call this when a Canadian user asks when income tax instalments are due or whether they have to pay instalments, as an individual (self-emp…`
- `get_quote`: `Call this when a user asks what it costs to get their business taxes or bookkeeping done, wants an accountant or tax preparer, or compares…`
- `get_sales_tax_registration`: `Call this when a user asks whether they need a sales tax permit, seller's permit or GST/HST/PST registration, what it's called, or which ag…`
- `list_required_documents`: `Call this when a user asks what documents or records they need to gather before getting their business taxes or bookkeeping done. Returns A…`
- `start_onboarding`: `Call this only after the user has explicitly said yes, in this chat, to sending their name, email and business details to Aldro to get thei…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://aldro.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
