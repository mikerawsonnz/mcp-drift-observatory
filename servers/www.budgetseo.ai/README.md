# www.budgetseo.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.budgetseo.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.budgetseo.ai/api/mcp` | 17 | [`5f820b4e030c`](32965d1328a8cdfe0cde.json) | 2026-11-02 |

## Tools at `https://www.budgetseo.ai/api/mcp`

- `check_keywords`: `Volume, difficulty, and intent for keywords the user names. Spends 2 lookup credits. Tell the user the cost and wait for a yes. At most 20…`
- `find_opportunities`: `Use for best opportunities across quick wins, research ideas, competitor gaps, rank drops, and AI Overview citation gaps. Filter with kinds…`
- `find_quick_wins`: `Use when the user asks for low-hanging fruit, quick wins, or striking-distance keywords. Each result includes the estimated monthly clicks…`
- `get_ai_visibility`: `Latest AI search snapshot and keywords where an AI Overview shows but does not cite the user. Pass projectId when the user has more than on…`
- `get_competitor_overview`: `Competitors and how many tracked keywords each one outranks the user on. Uses saved competitor data only and never starts a paid lookup. ke…`
- `get_keyword_action_plan`: `Deep context for one tracked keyword: ranking URL, history, SERP features, competitors, and a checklist. Use after a briefing when an agent…`
- `get_rank_changes`: `Winners and losers over a recent window. Use for what moved, what dropped, or a weekly review. days defaults to 7.`
- `get_search_performance`: `Real Google Search Console clicks, impressions, CTR, and average position for one project. Last 28 days, plus the previous 28 days. Does no…`
- `get_seo_briefing`: `Use this first when the user asks what to do with SEO today, what changed, or what to focus on. Returns the top actions, recent rank moves,…`
- `list_projects`: `List the user's BudgetSEO projects, keyword counts, whether a project is paused by the plan, and how many keyword slots remain.`
- `lookup_backlinks`: `Referring domains, backlink totals, and domain rank. Spends 3 lookup credits unless the result is already cached. Tell the user the cost an…`
- `lookup_domain`: `Organic keywords, estimated traffic, and top ranking URLs for a domain. Spends 4 lookup credits unless the result is already cached. Tell t…`
- `lookup_keywords`: `Keyword ideas from one seed: volume, difficulty, and intent. Spends 6 lookup credits unless the result is already cached. Tell the user the…`
- `research_keywords`: `Find new keyword ideas for one project. This spends AI research usage and is available on Starter and Pro. Confirm with the user first. The…`
- `track_keywords`: `Add keywords to a project. Does not spend lookup credits; it uses the plan keyword slots. Confirm the keywords with the user first. country…`
- `untrack_keyword`: `Remove one tracked keyword and its history. This cannot be undone. Confirm with the user before calling it.`
- `update_recommendation`: `Mark a briefing action done, dismissed, or snoozed. Call this after the user finishes or rejects an action so later briefings skip it. snoo…`

## Changes

- 2026-11-02: [schema changed](../../deltas/2026-11-02/32965d1328a8cdfe0cde.json): `38 field(s) changed`
- 2026-11-01: [count changed, schema changed, tool added](../../deltas/2026-11-01/32965d1328a8cdfe0cde.json): `1 tool(s) added; 46 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.budgetseo.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
