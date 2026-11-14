# mcp.ahel.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.ahel.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.ahel.ai` | 11 | [`432a4e0ff11a`](f81cefdfba92e36c524a.json) | 2026-11-14 |

## Tools at `https://mcp.ahel.ai`

- `balance`: `The workspace's prepaid balance, what running jobs have set aside, spending today and this month (for the Owner), any daily cap on this con…`
- `capability_inspect`: `One action by its id: its inputs, what it gives and its price rule. With arguments (the person's real inputs) it also prices that exact run…`
- `capability_run_status`: `Read a run that was still going: give execution_id from run_capability and results true for its rows. Answers the result in plain words, th…`
- `capability_search`: `Find the action for a job, by the person's own words ("work email of a person", "dentists in a city") or by an action id. Use it first for…`
- `catalog_request`: `Ask Ahel to add an action the catalog does not have, when capability_search finds nothing that fits. Give the job in plain words, one examp…`
- `feedback`: `Tell Ahel what went wrong or right: rate one run or request good or bad by its id, or with no id report anything confusing (results, charge…`
- `get_started`: `Start here when the person is new, asks what Ahel can do, or has no clear job yet. Answers what Ahel does in plain words, the ready-made re…`
- `review`: `Rate how useful one finished run was, after using its result: useful, partly, not_useful or not_sure, with an optional reason (missing rows…`
- `run_batch`: `Run one action over many inputs in one call (1 to 100 items, each the action's inputs), such as a company lookup for 20 domains. Priced the…`
- `run_capability`: `Run one action, after the person agreed to the price capability_inspect gave. Give id, arguments and max_cost_usd from that price: a run th…`
- `run_recipe`: `Run a recipe: a ready-made job of several actions, such as local businesses of one kind in one place with their emails (or only those with…`

## Changes

- 2026-11-14: [schema changed](../../deltas/2026-11-14/f81cefdfba92e36c524a.json): `1 field(s) changed; signals: length_more_than_doubled`
- 2026-11-13: [description changed](../../deltas/2026-11-13/f81cefdfba92e36c524a.json): `1 field(s) changed; signals: length_more_than_doubled`
- 2026-11-12: [annotation changed, description changed, field changed, schema changed, tool added, tool removed](../../deltas/2026-11-12/f81cefdfba92e36c524a.json): `1 tool(s) added; 1 tool(s) removed; 34 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.ahel.ai"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
