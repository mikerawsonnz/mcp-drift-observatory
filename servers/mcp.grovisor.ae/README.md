# mcp.grovisor.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.grovisor.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.grovisor.ae` | 8 | [`b517b1bc68ed`](6c75ae8ba62c19ecd7e3.json) | 2026-10-06 |

## Tools at `https://mcp.grovisor.ae`

- `grotax_compare_sbr`: `Compute the same facts with and without Small Business Relief (revenue ≤ AED 3m, periods ending by 31 Dec 2029). Shows tax payable and what…`
- `grotax_compute_ct`: `Estimate UAE Corporate Tax using the Grovisor computation (rows A–K): AED 375,000 0% band then 9%, 50% entertainment add-back, interest cap…`
- `grotax_get_rules`: `List every rate and threshold groTAX uses, with its legal source and whether it still needs verification (verify: true).`
- `grotax_health_check`: `Run the Grovisor CT reviewer red-flag checklist (SBR, free zone/QFZP, TP disclosure and Local/Master File, connected-person pay, related-pa…`
- `grotax_list_health_questions`: `List the groTAX health-check questions with their answer keys and allowed values, including which questions only apply after others (depend…`
- `grotax_penalties`: `Return and payment due date (9 months after period end) and estimated penalties: late filing AED 500 a month for 12 months then AED 1,000,…`
- `grotax_qfzp_de_minimis`: `Test whether a free zone company's non-qualifying revenue stays within the de minimis limit: the lower of 5% of total revenue or AED 5m (MD…`
- `grotax_tp_thresholds`: `Check which UAE transfer pricing documents apply: TP Disclosure Form (related-party transactions > AED 40m with a category > AED 4m, or con…`

## Changes

- 2026-10-06: [schema changed](../../deltas/2026-10-06/6c75ae8ba62c19ecd7e3.json): `42 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.grovisor.ae"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
