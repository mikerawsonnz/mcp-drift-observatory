# jawz.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/jawz.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://jawz.ai/api/mcp` | 22 | [`2045a609f47b`](b7dee41cc5b956811146.json) | 2026-09-08 |

## Tools at `https://jawz.ai/api/mcp`

- `get_chapter`: `Fetch the full content of a chapter by loop slug and node. Loops not marked open require entitlement; every published loop is currently ope…`
- `get_china_liquidity`: `Read the latest Mako-curated PBoC balance-sheet publication (CNY trillions + source URL + as_of_month + note). Public read — suitable for s…`
- `get_conditions_history`: `Financial-conditions read-history — a timeseries of how conditions have moved over recent weeks. Returns one row per sample date with the c…`
- `get_data_health`: `Freshness status for every data source Jawz reads: per-source release date, latest observation date, expected cadence, age in days, and whe…`
- `get_drift_alerts`: `Portfolio-wide drift scan. Iterates Decision Records, calls score_position_drift on each, returns flagged positions with severity + why_fla…`
- `get_etf_profile`: `ETF look-through for Chapter 2 Mode 2.2 (Concentration Check). Given ETF ticker(s), returns each fund's top holdings with weights so the AI…`
- `get_event_calendar`: `Scheduled US macro events (FOMC + CPI + NFP + PCE) with dates and consensus. Consensus values are Mako-curated and arrive with provenance (…`
- `get_financial_conditions`: `Full financial conditions read: global liquidity (Fed + ECB + BoJ central-bank balance sheets, FX-converted to USD; PBoC included when a fr…`
- `get_growth_indicators`: `Growth pillar indicators: industrial production (ISM proxy), consumer sentiment, yield curve, initial claims, plus the Atlanta Fed GDPNow n…`
- `get_inflation_indicators`: `Inflation pillar indicators: headline + core CPI, headline + core PCE (YoY and MoM), 5Y/10Y breakevens, wage growth. Returns classification…`
- `get_liquidity_history`: `Global-liquidity read-history — a timeseries of central-bank liquidity over recent weeks. Returns one row per sample date with the full dec…`
- `get_loop`: `Get metadata and chapter manifest for a loop by slug. Returns loop info and the list of chapter nodes with titles — no chapter content. All…`
- `get_macro_regime`: `Get current macro regime (GREEN/YELLOW/RED) with business cycle positioning. The response carries the same values three ways: 'presentation…`
- `get_prices`: `Live prices for one or more holdings. Resolves raw tickers (stocks, ETFs, crypto, international listings) and returns price, value, and day…`
- `get_regime_history`: `Macro regime read-history — a timeseries of how the regime and its drivers have moved over recent weeks. Returns one row per sample date (r…`
- `get_started`: `Orientation for a new Jawz connection, and for questions about what Jawz is, what it covers, or how it is used. Returns a description of th…`
- `get_weekly_data_releases`: `Past week's data releases with H.4.1 net liquidity update. Anchored to Friday — most current when run Friday morning or later. Each release…`
- `get_world_brief`: `Read the Jawz World Brief — the weekly Mako-bylined market read published at jawz.ai/brief. Returns the latest edition by default, or a spe…`
- `list_loops`: `List all available Jawz loops. Returns loop metadata, access status, and which loop is currently active for this user. Every published loop…`
- `run_chapter`: `Returns a chapter's published framework text: its modes, the questions each asks, and the output format it describes. The framework is refe…`
- `run_mode`: `Returns the published framework text for one named mode within a chapter, rather than the full chapter. Repeat calls return the same mode c…`
- `score_position_drift`: `Score how a single position's regime fit has drifted since entry. Returns regime_at_entry, regime_now, fit_score_at_entry, fit_score_now, d…`

## Changes

- 2026-09-08: [description changed](../../deltas/2026-09-08/b7dee41cc5b956811146.json): `3 field(s) changed; signals: length_more_than_doubled`
- 2026-09-07: [schema changed](../../deltas/2026-09-07/b7dee41cc5b956811146.json): `39 field(s) changed`
- 2026-09-01: [description changed, schema changed](../../deltas/2026-09-01/b7dee41cc5b956811146.json): `2 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**
- 2026-08-30: [description changed](../../deltas/2026-08-30/b7dee41cc5b956811146.json): `3 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://jawz.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
