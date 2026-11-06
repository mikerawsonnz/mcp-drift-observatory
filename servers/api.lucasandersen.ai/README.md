# api.lucasandersen.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.lucasandersen.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.lucasandersen.ai/mcp` | 6 | [`f9d488d6fa91`](fb07896b09a09a827d55.json) | 2026-08-20 |

## Tools at `https://api.lucasandersen.ai/mcp`

- `k1_basis_compute`: `Computes adjusted partner basis from a single year of Schedule K-1 data using the IRS Partner's Basis Worksheet methodology (Lines 1-14), p…`
- `k1_basis_multi_year`: `Computes a running adjusted partner basis across multiple years of Schedule K-1 data, per IRC §705 (basis computation), §731(a)(1) (gain on…`
- `mlp_estate_planning`: `Computes §1014 stepped-up basis and estate-planning analysis for one or more direct MLP positions held until death, per IRC §1014(a) (basis…`
- `mlp_info`: `Returns reference data for a supported MLP ticker — current cash distribution per unit, distribution growth CAGR, default return-of-capital…`
- `mlp_projection`: `Computes a multi-year tax projection for a publicly traded MLP position, applying the IRS Partner's Basis Worksheet methodology (Lines 1-14…`
- `mlp_sell_vs_hold`: `Compares selling an MLP position today (triggering §751(a) hot-asset ordinary recapture plus §731(a)(1) long-term capital gain) against hol…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.lucasandersen.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
