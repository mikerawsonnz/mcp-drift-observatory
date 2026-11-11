# beliefstate.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/beliefstate.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://beliefstate.ai/v1/research/mcp` | 23 | [`ae00b9ae2b9e`](d29176e06366706dabab.json) | 2026-11-11 |

## Tools at `https://beliefstate.ai/v1/research/mcp`

- `get_brief`: `Read a cited research brief for a covered U.S. ticker, ETF or released subject. Overview, current and full views support dated research and…`
- `get_case`: `Retrieves one complete investment case by returned belief_id: investor, reasoning, evidence, risks, catalysts, conditions, revisions, outco…`
- `get_cases`: `Retrieves dated investment cases for one company or research subject, with optional investor, direction and time filters. Returns attribute…`
- `get_catalysts`: `Retrieves evidence-linked catalysts for one company, research subject, investment case or the explicitly selected released corpus. Returns…`
- `get_changes`: `Retrieves the ordered research change journal for a company, subject, case or explicitly selected released corpus. Returns dated events, ci…`
- `get_companies`: `Find SEC-registered U.S. companies and selected verified international listings by symbol or name. Search by market, sector or exchange-qua…`
- `get_company_facts`: `Retrieves retained financial facts, company references, segment metrics, operating KPIs and management guidance for one ticker. Select reco…`
- `get_comparison`: `Retrieves a cited engine comparison of two distinct investment cases using their returned belief_id and compare_to_belief_id. Returns a cit…`
- `get_context_assessment`: `Retrieves a dated engine context assessment by its returned assessment identifier, including permitted supporting evidence and coverage lim…`
- `get_economic_calendar`: `Retrieves retained US economic events in one ticker research scope. Filter by event text, region, scheduled/reported/unconfirmed state and…`
- `get_insider_trades`: `Retrieves source-reported insider transactions for one ticker. Filter by reporting owner name or CIK, transaction codes, derivative status…`
- `get_institutional_holdings`: `Retrieves reported institutional holdings for one ticker across supported retained 13F history. Filter by manager name or CIK, report perio…`
- `get_investor_outcomes`: `Retrieves an investor's stored publication-based outcomes for one company, research subject, investment case or the explicitly selected rel…`
- `get_macro_context`: `Retrieves retained government macroeconomic observations in one ticker research scope. Filter by native series_ids, agency, measurement_nam…`
- `get_market_returns`: `Retrieves supported split-adjusted close-price returns for one ticker versus SPY. Request session_intervals from 1 to 252; date bounds sele…`
- `get_news`: `Check recent SEC filings for one verified ticker. Set include_earnings to also read issuer-announced earnings schedules when available. Fre…`
- `get_options_activity`: `Retrieves retained options bars, flow aggregates and open interest for one ticker. Select activity_type, call/put right, expiration, strike…`
- `get_risks`: `Retrieves evidence-linked risks for one company, research subject, investment case or the explicitly selected released corpus. Returns reco…`
- `get_search_results`: `Retrieves ranked published investment cases matching thesis, investment theme or trade setup, with an optional company or subject filter. R…`
- `get_short_activity`: `Retrieves retained short-interest and short-volume history for one ticker. Select family and date bounds; short_interest uses settlement pe…`
- `get_subjects`: `Retrieves matching released research subjects by name or kind, including companies, industries and investment themes. Returns matching subj…`
- `get_tickers`: `Retrieves public direct-company research coverage and counts. Account tracking requires the authenticated MCP server.`
- `get_visual`: `Retrieves saved research charts and tables for one investment case or context assessment. Without visual_id, returns available visual and r…`

## Changes

- 2026-11-11: [description changed, schema changed](../../deltas/2026-11-11/d29176e06366706dabab.json): `6011 field(s) changed; signals: length_more_than_doubled`
- 2026-11-10: [schema changed](../../deltas/2026-11-10/d29176e06366706dabab.json): `4959 field(s) changed; signals: length_more_than_doubled`
- 2026-11-09: [annotation changed, count changed, description changed, field changed, schema changed, tool added, tool removed](../../deltas/2026-11-09/d29176e06366706dabab.json): `20 tool(s) added; 15 tool(s) removed; 9574 field(s) changed; signals: length_more_than_doubled, url_introduced`
- 2026-11-08: [schema changed](../../deltas/2026-11-08/d29176e06366706dabab.json): `32408 field(s) changed; signals: length_more_than_doubled`
- 2026-11-06: [schema changed](../../deltas/2026-11-06/d29176e06366706dabab.json): `31954 field(s) changed; signals: length_more_than_doubled`
- 2026-11-05: [schema changed](../../deltas/2026-11-05/d29176e06366706dabab.json): `25644 field(s) changed; signals: length_more_than_doubled`
- 2026-11-04: [schema changed](../../deltas/2026-11-04/d29176e06366706dabab.json): `37864 field(s) changed; signals: length_more_than_doubled`
- 2026-11-03: [schema changed](../../deltas/2026-11-03/d29176e06366706dabab.json): `1 field(s) changed`
- 2026-11-02: [schema changed](../../deltas/2026-11-02/d29176e06366706dabab.json): `39227 field(s) changed; signals: length_more_than_doubled`
- 2026-11-01: [schema changed](../../deltas/2026-11-01/d29176e06366706dabab.json): `41414 field(s) changed`
- 2026-10-31: [schema changed](../../deltas/2026-10-31/d29176e06366706dabab.json): `36949 field(s) changed; signals: length_more_than_doubled`
- 2026-10-29: [description changed, schema changed](../../deltas/2026-10-29/d29176e06366706dabab.json): `16 field(s) changed`
- 2026-10-28: [description changed, schema changed](../../deltas/2026-10-28/d29176e06366706dabab.json): `40618 field(s) changed; signals: length_more_than_doubled`
- 2026-10-27: [count changed, tool added](../../deltas/2026-10-27/d29176e06366706dabab.json): `16 tool(s) added`
- 2026-10-26: [count changed, tool removed](../../deltas/2026-10-26/d29176e06366706dabab.json): `16 tool(s) removed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://beliefstate.ai/v1/research/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
