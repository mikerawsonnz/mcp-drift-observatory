# tax.brainy.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/tax.brainy.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://tax.brainy.ae/mcp` | 5 | [`a1eae710f205`](616941c9dc72ff71ada2.json) | 2026-11-26 |

## Tools at `https://tax.brainy.ae/mcp`

- `uae_einvoicing_dates`: `Compute UAE Accredited Service Provider (ASP) appointment and mandatory e-invoicing go-live dates from annual gross revenue and entity type…`
- `uae_einvoicing_penalty_estimate`: `Estimate UAE e-invoicing implementation administrative penalties under Cabinet Decision No. 173 of 2026, Annex item 1 (initial AED 5,000 pl…`
- `uae_quick_tax_estimate`: `Estimate UAE Corporate Tax (0% / 9% general bands, Qualifying Free Zone Person rates, or natural-person AED 1,000,000 business turnover thr…`
- `uae_tax_calendar`: `Generate a 12-month UAE business tax calendar (Corporate Tax return and first-period waiver deadlines, VAT201 deadlines with federal weeken…`
- `uae_vat_credit_expiry`: `Calculate the ordinary 5-year VAT credit deadline and the 31 December 2026 transitional refund or tax/penalty settlement window from the en…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://tax.brainy.ae/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
