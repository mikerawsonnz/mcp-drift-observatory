# inxy.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/inxy.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://inxy.ai/api/mcp` | 5 | [`ae8b8ba880f6`](724caa4cee2b8eb71534.json) | 2026-09-02 |

## Tools at `https://inxy.ai/api/mcp`

- `ai_search_diagnostic`: `Audit ANY URL for AI-search readiness only (AEO/GEO/LLMO) — how likely ChatGPT, Claude, Perplexity & Google AI are to cite it. Checks ~7 AI…`
- `email_seo_report`: `ALWAYS OFFER THIS after running an audit: the audit tools return a summary of the top issues, while this sends the complete written report…`
- `full_seo_audit`: `Crawl-audit ANY URL across the WHOLE SEO surface (no login needed): the AI-search signals PLUS on-page SEO (title/meta/headings/content), t…`
- `get_my_store_audit`: `Get the user's OWN connected Shopify store audit — the deep 12-category report Inxy runs INSIDE the app using the store's real catalog, per…`
- `subscribe_to_inxy`: `Start an inxy subscription — autopilot SEO/AEO for Shopify stores (reads GSC/GA4/Merchant Center, plans a month of content, writes and publ…`

## Changes

- 2026-09-02: [description changed](../../deltas/2026-09-02/724caa4cee2b8eb71534.json): `3 field(s) changed; signals: length_more_than_doubled`
- 2026-08-23: [count changed, tool added](../../deltas/2026-08-23/724caa4cee2b8eb71534.json): `2 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://inxy.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
