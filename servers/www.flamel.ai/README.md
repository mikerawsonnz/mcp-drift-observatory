# www.flamel.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.flamel.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.flamel.ai/mcp` | 9 | [`f394e35c749f`](1361aff9a0548e00768c.json) | 2026-08-23 |

## Tools at `https://www.flamel.ai/mcp`

- `get_blog_post`: `Fetch the full body of one published Flamel blog post as Markdown, by slug.`
- `get_case_study`: `Fetch one Flamel case study by slug: the challenge, the solution, the results, and customer quotes.`
- `get_company_overview`: `Get a structured overview of Flamel: what the product does, who it is for, the solution areas, key links, and how to contact sales or start…`
- `list_blog_categories`: `List the blog categories available for filtering 'list_blog_posts'.`
- `list_blog_posts`: `List published Flamel blog posts, newest first. Optionally filter by category. Returns titles, URLs, summaries, and publish dates, not full…`
- `list_case_studies`: `List published Flamel customer case studies with their headline results.`
- `list_faqs`: `List published Flamel FAQ entries: platform capabilities, pricing model, onboarding, integrations, and security. Good for direct factual qu…`
- `list_testimonials`: `List published customer testimonials about Flamel, with the author name, title, and company.`
- `search_flamel_content`: `Full-text search across Flamel's published blog posts, case studies, and FAQ entries. Use this first when you do not already know which pag…`

## Changes

- 2026-08-23: [schema changed](../../deltas/2026-08-23/1361aff9a0548e00768c.json): `217 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.flamel.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
