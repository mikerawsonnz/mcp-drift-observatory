# analyticslegends.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/analyticslegends.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://analyticslegends.ai/mcp` | 25 | [`9dfe896b5b2f`](44700875edd0c1c1f674.json) | 2026-11-11 |

## Tools at `https://analyticslegends.ai/mcp`

- `count_firms_by`: `Count the firm directory by country, region, kind, module or sap_signal_band, with search_firms' filters, instead of paging search_firms to…`
- `find_academy_modules`: `Search the Academy training catalogue (Datasphere, BDC, SAC, BW/4HANA, Databricks) by text, track or level. Rows are in the language asked.…`
- `find_answers`: `Start here for an SAP AI & analytics PROBLEM, asked in EN, FR or DE (agents in production, Joule value, BW 7.5 cliff, BDC vs Datasphere vs…`
- `find_opportunities`: `Search public SAP AI & analytics postings. Mostly PERMANENT roles: set employment_type for freelance questions. A posting listed in several…`
- `find_partner_candidates`: `Rank local service providers of a country or region as partner or acquisition candidates; local_only (default) excludes foreign groups' sub…`
- `find_sap_clients`: `Search the SAP END-CUSTOMER corpus (companies that run SAP); each row says its verification status. Paid: MCP Pass or Firm Pass key.`
- `get_academy_module`: `Read one Academy module in full (body, objectives, summary) by id or slug from find_academy_modules; 'lang' picks one language. Paid: MCP P…`
- `get_concept`: `One concept's metadata and editor's summary by slug from search_concepts (e.g. 'sap-business-data-cloud-bdc'). The card body, cheat sheet a…`
- `get_concept_card`: `The full concept card: body, cheat sheet, glossary, pro tip and the four analysis tables, EN/FR/DE. Paid: MCP Pass or Firm Pass key.`
- `get_day_rate_benchmark`: `Published SAP freelance day-rate aggregate by country, specialisation and seniority: min/max (median, p10, p90 when sourced) in the row's c…`
- `get_expansion_brief`: `Brief for entering a region: providers there (local vs group), SAP end-customer counts by country and industry, live opportunities, brand f…`
- `get_firm`: `One firm's public profile by its slug from search_firms (verbatim; some slugs are numeric). A brand name such as 'accenture' returns the li…`
- `get_firm_intel`: `Intelligence profile of a services firm: SAP practice size, partner level, products delivered, typical day rate, notable clients. Search by…`
- `get_sap_client_profile`: `One SAP end-customer's full profile (products in use, modules, analytics solutions, evidence) by id from find_sap_clients. Paid: MCP Pass o…`
- `get_study`: `Read a study's text: without 'section' returns the section list and introduction, then pass a heading as 'section'. Slugs from list_studies…`
- `list_firm_kinds`: `The organisation kinds of the firm directory with a live count each — the vocabulary of search_firms' 'kind'. Public, complete without a ke…`
- `list_freelance_platforms`: `Platforms where an SAP consultant can create a profile (freelance marketplaces, job boards, expert networks), with signup URL, confidence g…`
- `list_sap_modules`: `The SAP module/product taxonomy (codes such as DATASPHERE, BDC, SAC, BW4HANA with labels) that other tools filter on; use it to map loose w…`
- `list_studies`: `List the deep-research studies: title, edition, as-of date, audience, word count, citation_url, one row per study in the language asked. Me…`
- `query_knowledge_graph`: `Relations between concepts, Academy modules, studies and vendors: list nodes (node_type, query) or one node's edges (node_id). The only too…`
- `request_introduction`: `ACTION: a brief's anonymised selection, or with candidate_ref an introduction request the consultant answers in the app. Paid: MCP Pass or…`
- `search_concepts`: `Search the SAP AI & analytics concept encyclopaedia (the stack's vocabulary): slug, title, category, level, editor's summary. Full card: ge…`
- `search_firms`: `Search SAP AI & analytics service providers (consultancies, Big-4, agencies, SAP partners, platforms). Returns slug, name, HQ, website, cla…`
- `search_news`: `Search the curated SAP AI & analytics news corpus; defaults to SAP-specific items (scope 'sap'). Each item carries source_url (the publishe…`
- `submit_brief`: `ACTION: deposit an SAP need as a private brief, matched every 6 h against consenting consultants; nothing is e-mailed. Paid: MCP Pass or Fi…`

## Changes

- 2026-11-11: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-11-11/44700875edd0c1c1f674.json): `2 tool(s) added; 1131 field(s) changed`
- 2026-11-10: [description changed, schema changed](../../deltas/2026-11-10/44700875edd0c1c1f674.json): `3 field(s) changed`
- 2026-11-08: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-11-08/44700875edd0c1c1f674.json): `29 field(s) changed`
- 2026-11-07: [count changed, tool added](../../deltas/2026-11-07/44700875edd0c1c1f674.json): `1 tool(s) added`
- 2026-10-31: [description changed, schema changed](../../deltas/2026-10-31/44700875edd0c1c1f674.json): `12 field(s) changed`
- 2026-10-28: [description changed](../../deltas/2026-10-28/44700875edd0c1c1f674.json): `9 field(s) changed`
- 2026-10-26: [schema changed](../../deltas/2026-10-26/44700875edd0c1c1f674.json): `9 field(s) changed`
- 2026-10-25: [schema changed](../../deltas/2026-10-25/44700875edd0c1c1f674.json): `4 field(s) changed`
- 2026-10-24: [schema changed](../../deltas/2026-10-24/44700875edd0c1c1f674.json): `11 field(s) changed`
- 2026-10-19: [description changed, schema changed](../../deltas/2026-10-19/44700875edd0c1c1f674.json): `5 field(s) changed`
- 2026-10-13: [description changed](../../deltas/2026-10-13/44700875edd0c1c1f674.json): `1 field(s) changed`
- 2026-10-03: [schema changed](../../deltas/2026-10-03/44700875edd0c1c1f674.json): `5 field(s) changed`
- 2026-10-02: [description changed, schema changed](../../deltas/2026-10-02/44700875edd0c1c1f674.json): `3 field(s) changed`
- 2026-10-01: [annotation changed, count changed, description changed, field changed, schema changed, tool added](../../deltas/2026-10-01/44700875edd0c1c1f674.json): `2 tool(s) added; 38 field(s) changed`
- 2026-09-30: [annotation changed, description changed, field changed, schema changed](../../deltas/2026-09-30/44700875edd0c1c1f674.json): `17 field(s) changed`
- 2026-09-26: [schema changed](../../deltas/2026-09-26/44700875edd0c1c1f674.json): `3 field(s) changed; signals: length_more_than_doubled`
- 2026-09-25: [description changed, schema changed](../../deltas/2026-09-25/44700875edd0c1c1f674.json): `77 field(s) changed; signals: length_more_than_doubled`
- 2026-09-22: [description changed, schema changed](../../deltas/2026-09-22/44700875edd0c1c1f674.json): `3 field(s) changed`
- 2026-09-20: [description changed](../../deltas/2026-09-20/44700875edd0c1c1f674.json): `3 field(s) changed; signals: length_more_than_doubled`
- 2026-09-18: [description changed, schema changed](../../deltas/2026-09-18/44700875edd0c1c1f674.json): `68 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://analyticslegends.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
