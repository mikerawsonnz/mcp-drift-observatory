# ninar.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/ninar.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://ninar.ai/mcp` | 5 | [`22726671f45a`](2744c6059f3a976b2d63.json) | 2026-08-20 |

## Tools at `https://ninar.ai/mcp`

- `audit_brand_visibility`: `Check whether a brand or entity surfaced by an AI engine is a genuine competitor in your category (e.g. is 'Banner Life' actually a mortgag…`
- `generate_content`: `Generate AI-optimized content (FAQ, about copy, use cases, differentiators) for the gaps in your latest scan. Returns full content text inl…`
- `get_latest_score`: `Get the AI Visibility Index (0-100) for the signed-in user's most recently scanned brand, broken down by engine. Requires a free Ninar acco…`
- `list_content_gaps`: `List AI-generated content suggestions (FAQs, differentiators, use cases, about copy) the signed-in user can publish to close visibility gap…`
- `scan_visibility`: `Run an AI visibility scan for a brand. Pass 'city' for a local-business check (ChatGPT + Gemini, city-scoped). Omit 'city' for a multi-engi…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://ninar.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
