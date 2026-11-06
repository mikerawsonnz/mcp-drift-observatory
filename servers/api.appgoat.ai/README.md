# api.appgoat.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.appgoat.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.appgoat.ai/mcp` | 26 | [`9881ef918664`](9aff2500785fcb6529f4.json) | 2026-11-03 |

## Tools at `https://api.appgoat.ai/mcp`

- `apply_action`: `Go ahead with an action from propose_action, after the user has seen its diff and agreed. Outcomes: applied (written to the store / Apple A…`
- `audit_app`: `Run an App Audit of one app in one country: a 0–100 score, prioritised ASO actions with evidence, title / subtitle / keyword rewrites withi…`
- `get_action`: `One action from propose_action: its status (draft, pending_approval, approved, applied, failed, rejected), diff, guardrail scores, the prov…`
- `get_app`: `Look up one App Store or Google Play app: title, subtitle, developer, category, price, rating and histogram, installs (Play), version and d…`
- `get_app_changes`: `What changed in an app's store listing, newest first, with old and new values: version, release notes, title, subtitle, description, screen…`
- `get_app_history`: `An app's daily metric history per country: rating, ratings count, reviews count, installs (Play), star histogram and price, one row per day…`
- `get_app_keywords`: `The search terms an app ranks for in a country, best rank first, with popularity (5–100) and difficulty (0–100): from the weekly keyword un…`
- `get_audit`: `Check on an App Audit that audit_app started (by its id, e.g. aud_3fK9aQ2mXc81LpRt): waits up to about 25 s for it to finish, then returns…`
- `get_charts`: `A top free, paid or grossing chart for a store, country and category, today or on a past date: rank, app, developer, rating and the move si…`
- `get_competitors`: `An app's competitors, best first, scored from search terms both apps rank for (shared keywords) plus the store's similar-apps list. Feed th…`
- `get_developer`: `A developer's profile: name, website, country, app count, total ratings and installs, all their apps (most-rated first) and the same compan…`
- `get_events`: `Significant changes on your watched apps and keywords, newest first: type, one-line title, AI summary, significance (0–1), app, country and…`
- `get_insights`: `What an app's users praise and complain about, from the AI tags on its reviews: top issues (topics behind negative, bug, crash, UX and pric…`
- `get_job`: `Poll a background store fetch that another call started (its output said refreshing or still being fetched, with a job id): status, per-cou…`
- `get_keyword_ranks`: `Ranking history of a watched keyword: per capture the top 10 app ids, or with app, that app's rank over time (best, worst, latest). Default…`
- `get_reviews`: `Read an app's user reviews, newest first, up to 100 per page: rating, title, text, version, date, developer reply and AI tags (sentiment, i…`
- `keyword_research`: `Keyword metrics and research for App Store / Google Play search terms: popularity (5–100), difficulty (0–100), result count and the #1 resu…`
- `list_connections`: `The user's connected App Store Connect, Play Console and Apple Ads accounts: connection id, provider, mode (actions or read_only), status a…`
- `list_playbooks`: `AppGoat playbooks: step-by-step recipes (which tools to call, credit budget, decision rules, output format) for app audits, app idea resear…`
- `list_watches`: `Your watches (apps, competitor sets, keyword sets), newest first, with id, apps, terms, countries, event types and whether they are paused,…`
- `propose_action`: `Prepare a change to the user's connected account as a DRY RUN: nothing is written. AppGoat reads the live account and returns the before →…`
- `read_connection`: `Read live data from one of the user's connected accounts. what='reviews' (asc, play_console): the app's own reviews with reply status, unan…`
- `reject_action`: `Discard a draft or pending action the user does not want; nothing is written to the account. Cost: 0 credits.`
- `search_apps`: `Find apps by name or id in AppGoat's catalog of both stores (~5M apps): exact title matches first, then prefix, then substring, most-rated…`
- `unwatch`: `Stop watches by id (from list_watches or watch): no new events, and their watched apps and keyword slots are freed. Past events are kept. T…`
- `watch`: `Watch an app, a set of competitors or a set of keywords; significant changes become events (get_events, webhooks, daily email). kind app {a…`

## Changes

- 2026-11-03: [annotation changed](../../deltas/2026-11-03/9aff2500785fcb6529f4.json): `2 field(s) changed`
- 2026-10-28: [count changed, description changed, schema changed, tool removed](../../deltas/2026-10-28/9aff2500785fcb6529f4.json): `3 tool(s) removed; 2 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.appgoat.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
