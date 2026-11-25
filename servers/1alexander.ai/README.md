# 1alexander.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/1alexander.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://1alexander.ai/ai-visibility-tracker/api/mcp` | 17 | [`2041d361c647`](493ec4556eb754bc2406.json) | 2026-11-25 |

## Tools at `https://1alexander.ai/ai-visibility-tracker/api/mcp`

- `add_competitor`: `Track a competitor for a brand in the connected workspace, subject to workspace limits.`
- `add_prompt`: `Use list_brands to find brand_id. Add a tracked prompt (commercial by default) to a brand in your workspace. Use type branded for a questio…`
- `check_prompt`: `Queue a ChatGPT re-run of an active tracked prompt by exact brand name. Queues only when live checks are available and returns the request…`
- `competitor_gap`: `Find persisted answers where a recognized competitor is mentioned and your brand is absent. Optionally filter by competitor name.`
- `create_brand`: `Create a brand in the connected workspace, subject to workspace limits.`
- `get_account`: `Read plan, capacity, cadence and activity. No quota cost.`
- `get_citations`: `Return cited URLs, domains, titles and occurrence counts from persisted successful answers in your organization, ordered by count.`
- `get_prompt_answers`: `Read stored answers with named brands, deduplicated citations and answer text up to 4,000 characters by default. The truncated flag indicat…`
- `get_visibility`: `Summarize unbranded visibility and brand knowledge from saved answers. Return weekly mention rates, ranking, changes where prompt coverage…`
- `list_brands`: `List brands in your connected workspace with brand IDs, domains and tracked prompt counts, including inactive prompts.`
- `list_competitors`: `List only competitors manually tracked in the workspace for the selected brand. Brands merely mentioned in answers or shown on the Overview…`
- `list_engines`: `List engines and plan cadence.`
- `list_prompts`: `Use list_brands to find brand_id. List tracked prompts in your connected workspace, optionally restricted to a brand. Includes inactive pro…`
- `remove_competitor`: `Remove a tracked competitor while retaining stored answer evidence.`
- `suggest_prompts`: `Generate template prompt suggestions without running model calls or using tracked prompt slots. Adapt them and confirm wording with the use…`
- `update_brand`: `Update a workspace brand by ID, name or domain.`
- `update_prompts`: `Pause, resume or delete prompts. Delete requires confirm:true; otherwise returns the proposed deletions. Paused prompts consume capacity; d…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://1alexander.ai/ai-visibility-tracker/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
