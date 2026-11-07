# buildersinfintech.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/buildersinfintech.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://buildersinfintech.ai/mcp` | 31 | [`7576f158fa1a`](5838aac513603a4cf3ab.json) | 2026-11-07 |

## Tools at `https://buildersinfintech.ai/mcp`

- `about`: `What this database covers, how to cite it, and where the bulk downloads live.`
- `coverage_check`: `How many investors backed public fintech equity rounds in the last 12 months that match a country / stage / sub-sector, the top 3 investors…`
- `find_providers`: `Find companies by product category, licence (licensed_in matches the home country or any passported country), licence type, authority, and…`
- `funding_summary`: `Counts for a slice of the funding database: rounds, countries, totals per announced currency, undisclosed rounds and rounds per category. N…`
- `get_content`: `One published item by type and slug, with its body text (truncated), topics, countries, organizations and people. News items also include a…`
- `get_daily_digest`: `One edition of the Builders in Fintech daily digest (weekdays): the equity rounds that became public in its window (largest first within US…`
- `get_funding_index`: `The weekly Builders Fintech Funding Index of approved equity rounds (ISO weeks). Arguments: week (optional, 'YYYY-Www', e.g. '2026-W39') re…`
- `get_investor_scorecard`: `Follow-on scorecard for one investor by slug: of the portfolio companies it first backed at least the window ago, the share that raised a l…`
- `get_organization`: `Full public profile for one organization by slug: description, country, funding rounds (raised or led), people, any disclosure, editor_disc…`
- `get_person`: `Full public profile for one person by slug: bio, roles and coverage.`
- `get_product`: `Full public listing for one product by slug: description, category, markets, customer type, API, pricing model, links, the company and an a…`
- `get_report`: `One report by slug: publisher and co-publishers, date, type, gated flag, summary, up to 5 key figures (value and unit exactly as written, e…`
- `get_signals_report`: `The monthly Fintech Signals report: stored figures for approved equity rounds in one month (headline rounds and per-currency totals/medians…`
- `get_topic_digest`: `The weekly digest for one topic (currently the topics with a digest, e.g. 'stablecoins', 'agentic-payments'): published news tagged with th…`
- `largest_rounds`: `Largest disclosed equity rounds, ranked per currency (amounts are never converted between currencies).`
- `list_countries`: `Countries that have public coverage, with company and content counts.`
- `list_deploying_funds`: `Funds that raised in the last 24 months and are backing fintech rounds in the last 12: approved funds (not other-sector) whose latest first…`
- `list_events`: `Approved fintech events, upcoming by default, with optional country, format, topic and month filters.`
- `list_fund_closes`: `Approved venture-fund closes, newest first: fund, manager, close_type (launch, target, first, interim, final, unspecified), date, amount an…`
- `list_funding_rounds`: `Approved funding rounds, newest first, with optional filters and keyset pagination. Pass the returned next_cursor fields (after_date, after…`
- `list_provider_filters`: `Valid values for find_providers: product category slugs, licence type slugs, authority slugs, and the ISO codes of countries that have at l…`
- `list_raising`: `Fintech companies that pitched Builders in Fintech and opted in to a public listing while they raise: company name, website, one-liner, sta…`
- `list_topics`: `Every public topic with its slug and URL, for use as a filter in the other tools.`
- `most_active_investors`: `Investors ranked by the number of approved rounds they appear in. Category defaults to equity. With a country, only rounds of companies hea…`
- `search_content`: `Full-text search across published news, newsletter issues, podcast episodes, public entity pages, funding rounds and products. Result kinds…`
- `search_funds`: `Venture funds (fintech, partly fintech or generalist) with their manager, status, stages, latest close and size or target. Amounts are as a…`
- `search_organizations`: `Search fintech companies and investors by name, kind or country. Returns public profiles with canonical URLs. Arguments: q (or query): text…`
- `search_people`: `Search founders, operators and investors covered by the publication. Arguments: q (or query): text to search for, matched against the full…`
- `search_podcast_knowledge`: `Search attributed facts and question-and-answer pairs from Builders in Fintech podcast episodes (as stated by the guest, not independently…`
- `search_products`: `Search fintech products by text, category, market, API availability, agent access (has_mcp, has_sandbox, has_api) or customer type. Each pr…`
- `search_reports`: `Fintech reports, white papers, surveys and data, newest first, with publisher, type, date and gated flag. Reports are published by the comp…`

## Changes

- 2026-11-07: [count changed, tool added](../../deltas/2026-11-07/5838aac513603a4cf3ab.json): `2 tool(s) added`
- 2026-11-06: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-06/5838aac513603a4cf3ab.json): `4 tool(s) added; 9 field(s) changed`
- 2026-11-05: [count changed, description changed, schema changed, tool added](../../deltas/2026-11-05/5838aac513603a4cf3ab.json): `2 tool(s) added; 6 field(s) changed`
- 2026-11-03: [description changed](../../deltas/2026-11-03/5838aac513603a4cf3ab.json): `1 field(s) changed`
- 2026-10-28: [description changed, schema changed](../../deltas/2026-10-28/5838aac513603a4cf3ab.json): `5 field(s) changed`
- 2026-10-16: [count changed, description changed, tool added](../../deltas/2026-10-16/5838aac513603a4cf3ab.json): `2 tool(s) added; 2 field(s) changed`
- 2026-10-15: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-15/5838aac513603a4cf3ab.json): `1 tool(s) added; 9 field(s) changed`
- 2026-10-10: [description changed, schema changed](../../deltas/2026-10-10/5838aac513603a4cf3ab.json): `2 field(s) changed; signals: length_more_than_doubled`
- 2026-10-09: [count changed, tool added](../../deltas/2026-10-09/5838aac513603a4cf3ab.json): `1 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://buildersinfintech.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
