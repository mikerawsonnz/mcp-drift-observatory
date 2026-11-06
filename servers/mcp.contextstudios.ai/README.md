# mcp.contextstudios.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.contextstudios.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.contextstudios.ai/api/public/mcp` | 46 | [`1087bc2034db`](e74ea550d143e4aa4222.json) | 2026-10-02 |

## Tools at `https://mcp.contextstudios.ai/api/public/mcp`

- `ai_project_estimator`: `Interactive AI project estimation tool.`
- `blog_explorer`: `Interactive blog browsing interface.`
- `fetch`: `Fetch the full content of a document by ID returned from the search tool (e.g. 'blog:de:mein-artikel'), OR by a full https://www.contextstu…`
- `find_local_ai_recipes`: `Recommend local-AI setups for a given hardware: platform + device count, optional goal (quality / balance / speed). Returns the editorial p…`
- `get_blog_posts`: `Search and retrieve published blog posts.`
- `get_company_info`: `Retrieve comprehensive information about Context Studios including company overview, tech stack, differentiators, legal info, and contact d…`
- `get_company_type`: `Get a specific company-size segment's full profile: name, TL;DR, entity definition, description, characteristics/needs, FAQ, and canonical…`
- `get_comparison`: `Retrieve a detailed comparison between two AI tools.`
- `get_faq`: `Get frequently asked questions. 'scope=site' (default) returns the general Context Studios FAQ. 'scope=service' or 'scope=industry' require…`
- `get_featured_glossary_terms`: `Get a curated list of featured AI terms.`
- `get_glossary_by_tech_stack`: `Filter glossary terms by technology provider or stack.`
- `get_glossary_term`: `Get a detailed explanation of an AI term.`
- `get_guide`: `Get a specific guide.`
- `get_industry`: `Get a specific industry's full profile: name, TL;DR, entity definition, description, typical pain points, FAQ, and canonical + Markdown-twi…`
- `get_local_ai_creator`: `Get one creator with all of their published local-AI recipes (numbers with category, condition, source_url).`
- `get_local_ai_methodology`: `How the local-AI hub measures and ranks: categories (typ = everyday, mixed, peak), rank formula, E12 rule (values of some third-party sites…`
- `get_local_ai_quality`: `Agentic quality results for local models from Terminal-Bench-Mini (core19) by kyuz0, Apache-2.0: pass rate within attempts and pass@1 per m…`
- `get_local_ai_recipe`: `Get one published local-AI recipe by slug: all measured numbers (each with category, condition, source_url), weights with licenses, sources…`
- `get_location_page`: `Get specific location page.`
- `get_page`: `Get a specific CMS page by slug and locale.`
- `get_pricing_model`: `Explain how Context Studios prices projects: the entry point is a fixed-price workshop (Light Discovery, Strategy Day, or Prototyping Sprin…`
- `get_related_glossary_terms`: `Get terms that are related to a specific glossary term.`
- `get_role`: `Get a specific role's full profile: name, TL;DR, entity definition, description, responsibilities, FAQ, and canonical + Markdown-twin URLs.`
- `get_services`: `List the services offered by Context Studios. Every service sits under one of six goals (cluster) and is delivered in one or more of four f…`
- `get_use_case`: `Get a specific use case's full profile: name, TL;DR, entity definition, description, key features/benefits, FAQ, and canonical + Markdown-t…`
- `get_workshops`: `Get the three fixed-price entry workshops (Light Discovery, Strategy Day, Prototyping Sprint) with price, duration, and delivery mode, plus…`
- `list_company_types`: `List the company-size segments Context Studios serves (e.g. startups, SMB, enterprise), with name, one-line summary, and canonical + Markdo…`
- `list_comparisons`: `List all available comparisons.`
- `list_glossary_categories`: `List all 10 glossary categories.`
- `list_guides`: `List public guides.`
- `list_industries`: `List the industries Context Studios serves, with name, one-line summary, and canonical + Markdown-twin URLs.`
- `list_local_ai_creators`: `List the creators (people/projects) behind the published local-AI recipes, with recipe counts per platform.`
- `list_local_ai_hardware`: `Hardware platforms of the local-AI hub with datasheet (memory, bandwidth, TDP — each with vendor source) and current German prices (EUR inc…`
- `list_local_ai_recipes`: `List published local-AI recipes (model + quantization + engine on specific hardware: DGX Spark, Mac, Strix Halo, RTX 3090/5090/PRO 6000) fr…`
- `list_location_pages`: `List public location and bundesland pages.`
- `list_roles`: `List the buyer/user roles Context Studios addresses (e.g. founder, CTO, marketing manager), with name, one-line summary, and canonical + Ma…`
- `list_use_cases`: `List the software use cases Context Studios builds (e.g. CRM, invoicing, booking systems), with name, one-line summary, and canonical + Mar…`
- `request_consultation`: `Request a free consultation with Context Studios. Use this when a user wants to get in touch, start a project, or receive an offer. Capture…`
- `search`: `Search all public Context Studios content (blog, guides, glossary, AI comparisons). Returns result IDs for use with the fetch tool.`
- `search_blog_knowledge`: `Deep full-text search through the entire blog knowledge base. Provide either 'query' (full-text search) or 'slug' (fetch a specific post).`
- `search_comparisons`: `Search comparisons by keyword.`
- `search_content`: `Universal search across all public content.`
- `search_glossary`: `Search the AI glossary by keyword or category. Provide either 'query' or 'category'.`
- `search_guides`: `Search public guides.`
- `search_location_pages`: `Search public location and bundesland pages.`
- `search_pages`: `Full-text search across all published CMS pages.`

## Changes

- 2026-10-02: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-02/e74ea550d143e4aa4222.json): `8 tool(s) added; 24 field(s) changed; signals: length_more_than_doubled`
- 2026-09-26: [count changed, description changed, field changed, schema changed, tool added, tool removed](../../deltas/2026-09-26/e74ea550d143e4aa4222.json): `11 tool(s) added; 1 tool(s) removed; 229 field(s) changed; signals: length_more_than_doubled, url_introduced`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.contextstudios.ai/api/public/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
