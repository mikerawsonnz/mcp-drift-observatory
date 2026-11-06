# www.dsght.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.dsght.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.dsght.ai/mcp` | 10 | [`47cfe12466b4`](e12aa8635aacca92f972.json) | 2026-10-12 |

## Tools at `https://www.dsght.ai/mcp`

- `detect_tensions`: `Use when the user pastes strategy text and asks what is internally inconsistent: detects the structural contradictions — where the text qui…`
- `extract_assumptions`: `Use when the user pastes a strategy, plan, or memo and wants its hidden bets made explicit: extracts the falsifiable, load-bearing assumpti…`
- `get_country_indicator`: `Look up a country's authoritative macro indicator (inflation / gdp_growth) directly — deterministic, offline, cited. Use whenever you need…`
- `get_public_report`: `Get the latest full foresight report (markdown) for a published future-space. Use when the user wants the detailed analysis, or a quotable,…`
- `get_public_scenarios`: `Get the scenario matrix with probabilities for a published future-space. Use when the user asks how a domain (banking, energy, CEE markets,…`
- `get_public_tensions`: `Get the structural tensions — the load-bearing contradictions — for a published future-space. Use when the user asks what forces conflict,…`
- `list_countries`: `List the jurisdictions and macro indicators (inflation, GDP growth) available to resolve_country_claim and get_country_indicator, with per-…`
- `list_public_spaces`: `List the DSGHT future-spaces published for public use (slug, topic, status, depth). Call this first to discover what foresight is available…`
- `resolve_country_claim`: `Use this WHENEVER the user states or asks you to verify a numeric macro claim (inflation, GDP, interest rates): settle it against the claim…`
- `search_spaces`: `Find the most relevant published DSGHT future-space by keyword (topic + report text, plain-text ranked, no AI). Use this to locate a space…`

## Changes

- 2026-10-12: [annotation changed, field changed](../../deltas/2026-10-12/e12aa8635aacca92f972.json): `60 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.dsght.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
