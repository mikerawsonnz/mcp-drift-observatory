# betterpost.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/betterpost.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://betterpost.ai/mcp` | 23 | [`875ad5721337`](229d08d9b0c396cb5176.json) | 2026-08-20 |

## Tools at `https://betterpost.ai/mcp`

- `betterpost_add_source`: `Adds a source to a project and fetches it immediately (bounded by a few seconds), returning 'storiesAdded' so the next generate_content can…`
- `betterpost_add_story`: `Manually imports a story you read about from its URL (pinned relevance, flagged is_manual) so generation can draw on it.`
- `betterpost_create_project`: `Create a content project. Slow, one-shot: infers config (criteria, industry, tone), discovers sources, and gathers/ranks an initial set of…`
- `betterpost_delete_content`: `Delete a piece of content and its hosted images.`
- `betterpost_delete_project`: `Permanently deletes a project and everything in it — its sources, stories, and content. Cannot be undone.`
- `betterpost_derive_content`: `Transform an existing piece into another format (e.g. newsletter → tweet). No fetching; reuses the source stories and topic.`
- `betterpost_expand_coverage`: `Broadens a project's coverage: expands the relevance criteria (when needed), finds more sources across news, the web, and the relevant soci…`
- `betterpost_generate_content`: `Generate a new piece of content for a project from its timely, relevant stories. Fast in steady state. Charges credits on success only. If…`
- `betterpost_get_content`: `Fetch one piece of content in full.`
- `betterpost_get_project`: `Returns one project with its relevance 'criteria' (each with an id, so a criterion can be targeted for removal via betterpost_update_projec…`
- `betterpost_get_settings`: `Returns a project's per-content-type settings (wordLimit and additionalInstructions for each channel).`
- `betterpost_get_usage`: `Your credit balance, freeze state, and recent spend.`
- `betterpost_hide_story`: `Hides a story so generation ignores it. Reversible with unhide_story.`
- `betterpost_humanize`: `Rewrite existing text into BetterPost's readable, human voice. Preserves the meaning, facts, links, and format; returns the rewritten text…`
- `betterpost_list_content`: `List a project's content (summaries + shareable 'publicUrl' links).`
- `betterpost_list_projects`: `Returns your projects, each with its relevance 'criteria' (with ids) that define what counts as on-topic.`
- `betterpost_list_sources`: `Returns one slimmed page of a project's sources plus project-wide 'total' and 'counts' (ok/failing/disabled/pending, and byType). Page with…`
- `betterpost_list_stories`: `Returns a project's gathered stories, each with 'title', 'url', 'summary', 'relevancy', 'publicationDate', and 'isManual'/'isHidden' flags.…`
- `betterpost_remove_source`: `Removes a source from a project. Its already-gathered stories stay; the source is no longer fetched.`
- `betterpost_suggest_topics`: `Clusters a project's current stories into a few candidate angles — each with a label, how many stories back it, and example headlines — and…`
- `betterpost_unhide_story`: `Unhides a previously hidden story so generation can use it again.`
- `betterpost_update_project`: `Updates a project's title, audience, description, tone, freshness window, timezone, or relevance criteria, and returns the updated project…`
- `betterpost_update_settings`: `Patches one content type's wordLimit and/or additionalInstructions (free-form writing guidance for that type; pass an empty string to clear…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://betterpost.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
