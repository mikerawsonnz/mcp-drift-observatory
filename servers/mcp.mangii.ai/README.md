# mcp.mangii.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.mangii.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.mangii.ai/mcp` | 9 | [`4a631ea66584`](9a75041193e6f8bc90f8.json) | 2026-08-24 |

## Tools at `https://mcp.mangii.ai/mcp`

- `manga.buy_credits`: `Return the Console billing URL so a human can fund apiPackCredits. Generate-scoped keys cannot create Checkout sessions. Call this after 40…`
- `manga.continue_story`: `Add the next panel. Do not send style_id. Defaults: Image 1 = first panel (identity), Image 2 = last distinct panel (scene). Override via m…`
- `manga.create_story`: `Start a new private manga (panel 1). Required: prompt + style_id from manga.list_styles. Optional identity_image or reference_image is Imag…`
- `manga.get_credits`: `Return the API wallet. Spendable is apiPackCredits plus purchase-backed packCredits. weeklyCredits is display-only and does not pay MCP or…`
- `manga.get_job`: `Poll a generation job from manga.create_story, manga.continue_story, or manga.regenerate_panel when async=true. Repeat until status is succ…`
- `manga.list_panels`: `List panels you own for a story. Use this to get panel_id values before changing Image 1 or Image 2 on manga.continue_story or manga.regene…`
- `manga.list_stories`: `List stories you own, newest first. Call this when you lost story_id after context compaction so you can resume with manga.continue_story.…`
- `manga.list_styles`: `List the 24 canonical Mangii art styles with live style ids. Call this before manga.create_story. Experimental and alias ids are excluded.…`
- `manga.regenerate_panel`: `Redraw or edit one panel. Style stays locked. Same Image 1 / Image 2 ref overrides as manga.continue_story. Get ids from manga.list_panels.…`

## Changes

- 2026-08-24: [count changed, description changed, schema changed, tool added](../../deltas/2026-08-24/9a75041193e6f8bc90f8.json): `2 tool(s) added; 50 field(s) changed; signals: imperative_language_introduced, length_more_than_doubled` **(notable)**

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.mangii.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
