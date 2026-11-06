# childadhd.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/childadhd.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://childadhd.ai/api/mcp/v1` | 6 | [`bd305708c505`](7247ac0f9840d7d4f907.json) | 2026-08-20 |

## Tools at `https://childadhd.ai/api/mcp/v1`

- `cite_article`: `Get a formatted citation for a ADHD in Children article. Supports AMA, APA, and Chicago styles.`
- `get_article`: `Fetch a single article from ADHD in Children by slug. Returns title, body content, author, clinical reviewer, citations, and metadata.`
- `get_crisis_resources`: `Return the canonical 988 / 911 / Crisis Text Line payload. Surface this immediately whenever the user signals self-harm or imminent danger.`
- `get_microsite_info`: `Identity and links for ADHD in Children: tagline, audience, focus, publisher, sponsor relationship to Emora Health, and key URLs.`
- `list_articles`: `Paginated list of articles from ADHD in Children. Returns title, slug, summary, and URL.`
- `search_articles`: `Search ADHD in Children's editorial corpus by query. Returns title, slug, summary, and URL for matching articles.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://childadhd.ai/api/mcp/v1"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
