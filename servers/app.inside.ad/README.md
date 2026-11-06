# app.inside.ad: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.inside.ad.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.inside.ad/api/mcp` | 3 | [`25af73bef4c9`](840468f62d79747af8ce.json) | 2026-08-28 |

## Tools at `https://app.inside.ad/api/mcp`

- `create_campaign_draft`: `Build a ready-to-launch ad campaign for a product WITHOUT the user having an account yet. Parses the landing page, generates ad creatives,…`
- `estimate_campaign`: `Estimate reach, clicks and cost of advertising a product to Telegram audiences — no account or authorization required. Call this FIRST, bef…`
- `get_draft_status`: `Check what happened to a campaign draft you created with create_campaign_draft: whether the user opened the link, signed in and paid. Poll…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.inside.ad/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
