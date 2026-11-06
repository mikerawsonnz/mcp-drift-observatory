# lumify.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/lumify.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://lumify.ai/mcp` | 24 | [`ba2b80e3998c`](f54f9bfdeab46c79c376.json) | 2026-09-03 |

## Tools at `https://lumify.ai/mcp`

- `batch_get_events`: `Get multiple events by id in one call — for agents that already have a list of ids and want full detail for each without one call per event…`
- `estimate_cost`: `Estimate the credit cost of one or more planned tool calls before making them — no credits are spent. Costs are data-dependent (e.g. odds/i…`
- `get_event`: `Get a single event with participants and venue. Optionally inline current odds and/or bet intelligence (same 1 credit as the event call). R…`
- `get_intelligence`: `Get predictive bet intelligence for an event: vig-stripped probability, fair_price, Price overlay, main-line ev (Beta), and forecasts[] — f…`
- `get_live_score`: `Get a lightweight live score snapshot for an event: status, period, clock, per-participant score and period-by-period scores, and last-upda…`
- `get_odds`: `Get current betting odds for an event: per-bookmaker lines and last-updated time. Includes in-play quotes while the event is underway; book…`
- `get_odds_history`: `Get line-movement history for an event: a list of past odds snapshots (movements), each with its own timestamp, up to limit entries. bookma…`
- `get_period_odds`: `Get first-half / first-five / first-set lines and live progress for an NFL, NCAAF, NBA, NCAAB, MLB, soccer, or tennis event. Joins persiste…`
- `get_player`: `Get a single player identity profile: name, sport, country, position/handedness, physical stats, current team, rankings (tennis {singles, p…`
- `get_player_events`: `List a player's events (schedule/results), paginated by id (after_id). Defaults to ±30 days around today when no date filter is given. Reso…`
- `get_player_props`: `Get player-prop lines and live progress for an NFL, NCAAF, NBA, NCAAB, NHL, or MLB event. Joins persisted player-prop mains to this-event p…`
- `get_prediction_markets`: `Get prediction-market game-line probabilities for an NFL, NCAAF, NBA, NHL, MLB, soccer, or tennis event. Persist-then-read from Fanatics Ma…`
- `get_splits`: `Get public betting splits (bets% and handle%) for an event: a consensus split plus a per-bookmaker breakdown (bookmakers[].bookmaker uses t…`
- `get_stats`: `Get raw, deterministic team/match statistics for a soccer, MLB, tennis, NFL, NCAAF, NBA, NCAAB, or NHL event — no odds (use get_odds) and n…`
- `get_team`: `Get a single team profile with its home venue. Raises a not-found error if team_id doesn't exist. Resolve ids via list_teams.`
- `get_team_props`: `Get team-total lines and live progress for an NFL, NCAAF, MLB, or soccer event. Joins persisted Pinnacle team-total mains (each team's full…`
- `list_ev`: `Beta. List pregame main-line +EV opportunities for a predictive-framework sport (soccer, mlb, tennis, nfl, ncaaf), sorted by ev_pct descend…`
- `list_events`: `List events (schedules and live scores), paginated by id (after_id). Filter by sport, league, status, date range, season, or team_id (resol…`
- `list_forecasts`: `Daily board of forecasted wagers from Lumify's model — a prediction, not a beat-the-market claim (no OOS/independence gate; see list_ev for…`
- `list_seasons`: `List seasons per sport/league. By default returns only currently active seasons; pass current_only=false to include historical seasons. Opt…`
- `list_sports`: `List supported sports with their leagues and current season. Returns each sport's id, slug, name, team-sport flag, and its leagues (each wi…`
- `list_teams`: `List teams, paginated by id (after_id). Filter by sport, league, conference, division, country, active status, or name (q, partial match).…`
- `query_events`: `Search events with a natural-language query instead of structured filters — e.g. 'live nfl games today' or 'college basketball this week'.…`
- `search_players`: `Search players by name, sport, country, ranking, or active status, paginated by id (after_id). Returns the same identity object on every sp…`

## Changes

- 2026-09-03: [count changed, schema changed, tool added](../../deltas/2026-09-03/f54f9bfdeab46c79c376.json): `1 tool(s) added; 14 field(s) changed`
- 2026-08-31: [schema changed](../../deltas/2026-08-31/f54f9bfdeab46c79c376.json): `2 field(s) changed`
- 2026-08-30: [description changed, schema changed](../../deltas/2026-08-30/f54f9bfdeab46c79c376.json): `73 field(s) changed; signals: length_more_than_doubled`
- 2026-08-29: [count changed, description changed, schema changed, tool added](../../deltas/2026-08-29/f54f9bfdeab46c79c376.json): `1 tool(s) added; 159 field(s) changed; signals: length_more_than_doubled, url_introduced`
- 2026-08-27: [description changed, schema changed](../../deltas/2026-08-27/f54f9bfdeab46c79c376.json): `8 field(s) changed; signals: url_introduced`
- 2026-08-26: [description changed, schema changed](../../deltas/2026-08-26/f54f9bfdeab46c79c376.json): `14 field(s) changed`
- 2026-08-25: [count changed, description changed, schema changed, tool added](../../deltas/2026-08-25/f54f9bfdeab46c79c376.json): `1 tool(s) added; 8 field(s) changed; signals: url_introduced`
- 2026-08-24: [count changed, description changed, schema changed, tool added](../../deltas/2026-08-24/f54f9bfdeab46c79c376.json): `2 tool(s) added; 7 field(s) changed`
- 2026-08-23: [description changed, schema changed](../../deltas/2026-08-23/f54f9bfdeab46c79c376.json): `7 field(s) changed; signals: imperative_language_introduced` **(notable)**
- 2026-08-22: [count changed, description changed, schema changed, tool added](../../deltas/2026-08-22/f54f9bfdeab46c79c376.json): `1 tool(s) added; 3 field(s) changed; signals: url_introduced`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://lumify.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
