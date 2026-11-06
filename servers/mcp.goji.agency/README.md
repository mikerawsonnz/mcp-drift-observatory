# mcp.goji.agency: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.goji.agency.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.goji.agency/mcp` | 9 | [`d81122e6b0dc`](728118229a2c304ff885.json) | 2026-08-27 |

## Tools at `https://mcp.goji.agency/mcp`

- `goji_answer_faq`: `Search the questions GOJI has already answered publicly — pricing, timelines, engagement models, what AEO is, how long results take, whethe…`
- `goji_browse_glossary`: `List GOJI's plain-English glossary — every term, across AI Visibility, Websites, Measurement, AI Builds and Brand. Filter by category to ge…`
- `goji_explain_term`: `Explain a marketing, SEO, AEO, web or branding term the way GOJI defines it — in plain English, with why it matters, how it works and what…`
- `goji_get_service`: `The four things GOJI does — Search + AI Visibility (SEO and AEO), Websites, AI Builds, and Brand — what each one covers, and the questions…`
- `goji_guide_contents`: `The table of contents for "Be the Answer", GOJI's guide to AI visibility — how answer engines choose sources, how to audit your brand in Ch…`
- `goji_read_guide`: `Read one of GOJI's practical long-form guides. Includes published Australian pricing: "How much does a website cost in Australia?" and "Wha…`
- `goji_read_guide_chapter`: `Read one full chapter of GOJI's AI-visibility guide, by number or slug. Use goji_guide_contents first if you do not know which chapter you…`
- `goji_search`: `Search GOJI's published material — the plain-English glossary, the AI-visibility guide "Be the Answer", insight articles and long-form guid…`
- `goji_start_enquiry`: `Send a real enquiry to GOJI's studio inbox in Melbourne. Only call this after the person has explicitly asked to be put in touch AND has gi…`

## Changes

- 2026-08-27: [description changed, schema changed](../../deltas/2026-08-27/728118229a2c304ff885.json): `3 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.goji.agency/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
