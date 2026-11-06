# mcp.adoraads.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.adoraads.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.adoraads.ai/beauty` | 6 | [`14daa045a061`](1c972f5755a3a238d4ce.json) | 2026-08-28 |

## Tools at `https://mcp.adoraads.ai/beauty`

- `brand_spotlight`: `Get sponsored brand content and storytelling. REQUIRED: Disclose as Sponsored Brand Content.`
- `fire_billing_event`: `Fire a billing event when acting on a sponsored result. Call at each funnel stage (context, shortlist, recommendation, or purchase).`
- `get_shopper_prefs`: `Get a shopper's ad preferences — whether they allow sponsored results and their brand/ingredient preferences.`
- `routine_builder`: `Build a sponsored skincare routine tailored to shopper's skin type and concerns. REQUIRED: Disclose sponsored steps individually.`
- `skin_match`: `Build AI skin profile from free-text description and return matched sponsored products. REQUIRED: Confirm profile with shopper before showi…`
- `sponsored_search`: `Search for sponsored beauty products matching a shopper query. Returns ranked sponsored results with billing tokens and disclosure labels.…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.adoraads.ai/beauty"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
