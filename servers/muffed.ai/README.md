# muffed.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/muffed.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://muffed.ai/api/mcp` | 14 | [`0aa41f93aa77`](86f65b26881f8d465f88.json) | 2026-08-22 |

## Tools at `https://muffed.ai/api/mcp`

- `compare_entities`: `Two players or two teams shown side by side, on the metrics that matter for their position by default — name metrics explicitly, or pass al…`
- `get_backfield`: `Muffed's published handcuff page for one team's backfield, plus the current depth chart and injury status from Sleeper. Answers who backs u…`
- `get_current_insights`: `Muffed's published editorial reads on what is real in the NFL right now — each one a dated, sourced claim with its supporting figures, from…`
- `get_entity_metrics`: `Every verified figure Muffed holds for one NFL player or one NFL team (by name or abbreviation, e.g. "Bijan Robinson" or "DEN"), with the s…`
- `get_metric_definition`: `Muffed's published definition of a verified metric — what it measures, in plain language, from the glossary page for that term — plus which…`
- `list_metrics`: `What Muffed can answer on. By default a summary of metric families with their counts and season coverage; pass search or detail:true for in…`
- `query_stat_leaders`: `Top entities on one verified metric for one season, pre-sorted, each with the source's own rank and the population it was ranked against. C…`
- `run_stat_query`: `Call this for any question about NFL statistics, leaders, rankings, splits, career or team spans, or how a player or team compares to other…`
- `sleeper_find_leagues`: `Lists the NFL leagues a Sleeper username belongs to, so a league id can be picked for the other league tools. Muffed stores nothing about w…`
- `sleeper_get_league`: `One league's name, season, size, current week, detected scoring format, and the manager-to-roster map. Everything downstream reads better o…`
- `sleeper_matchup_preview`: `Both sides of a league matchup, with the verified figures Muffed holds for the players involved and each team's record. Muffed does not pro…`
- `sleeper_roster_stories`: `One team's roster mapped to the verified figures and published Muffed surfaces for each player. Players Muffed does not cover are listed as…`
- `sleeper_standings_story`: `League standings derived from Sleeper's roster settings — records, points for, and points against where available. Sleeper publishes no sta…`
- `verify_claim`: `Checks structured claims against Muffed's verified panel. Each claim comes back confirmed, wrong (with the actual value), or unverifiable (…`

## Changes

- 2026-08-22: [description changed, schema changed](../../deltas/2026-08-22/86f65b26881f8d465f88.json): `5 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://muffed.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
