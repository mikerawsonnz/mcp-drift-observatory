# analyticslegends.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/analyticslegends.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://analyticslegends.ai/mcp` | 23 | [`f01427876780`](44700875edd0c1c1f674.json) | 2026-11-07 |

## Tools at `https://analyticslegends.ai/mcp`

- `count_firms_by`: `Answer a COUNTING question about the published firm directory in one call: how many organisations per country, per REGION (the six-value ge…`
- `find_academy_modules`: `Search the Analytics Legends Academy — the written training modules on SAP Datasphere, Business Data Cloud, SAP Analytics Cloud, BW/4HANA a…`
- `find_answers`: `Start here when someone asks about an SAP AI & analytics PROBLEM rather than a term. Matches a natural question, in English, French or Germ…`
- `find_opportunities`: `Search every SAP contract and permanent-role posting Analytics Legends publishes to an ANONYMOUS visitor. Only the SITE RADAR leg below is…`
- `find_partner_candidates`: `Rank the LOCAL service providers of a target country or region — the firms a practice partners with, subcontracts to, or acquires to enter…`
- `find_sap_clients`: `Search the SAP END-CUSTOMER corpus — the companies that RUN SAP, not the firms that sell services (those are search_firms). This is the pai…`
- `get_academy_module`: `Read one Academy training module in full — body, learning objectives and summary, EN, FR and DE — the written course corpus the Consultant…`
- `get_concept`: `Fetch one concept entry by slug: title, category, level, tags and the editor's summary. Written by a named human editor, not generated. 'le…`
- `get_concept_card`: `The FULL encyclopaedia card for one concept — body, cheat sheet, glossary, pro tip, and the four analysis tables (decision table, peer comp…`
- `get_day_rate_benchmark`: `The PUBLIC day-rate aggregate for SAP AI & analytics freelance work: min/max daily rate by country, specialisation and seniority — 'daily_r…`
- `get_expansion_brief`: `The one-call brief a services practice reads before opening a subsidiary in another region: providers already there (by kind and by country…`
- `get_firm`: `Fetch one organisation from the published directory by its database slug ('rows[].slug' from search_firms, verbatim). Returns the same publ…`
- `get_firm_intel`: `The paid intelligence profile of a services firm — SAP practice size and partner level, delivery flags per product, typical day rate and se…`
- `get_sap_client_profile`: `The full profile of one SAP end-customer — SAP footprint (products in use, modules known), analytics solutions, identity and evidence field…`
- `get_study`: `Read one Analytics Legends study BODY — the paid text behind list_studies' metadata. Requires the API key of an MCP Pass or Firm account (t…`
- `list_firm_kinds`: `Breakdown of the published firm directory by organisation kind, with a live row count per kind. Use this before search_firms to know what t…`
- `list_freelance_platforms`: `The subset of the published directory where a consultant can CREATE A PROFILE — freelance marketplaces, job boards with candidate profiles,…`
- `list_sap_modules`: `The canonical SAP module/product taxonomy Analytics Legends classifies against (codes and EN/FR labels by category). Use it to normalise a…`
- `list_studies`: `List the Analytics Legends deep-research studies with their edition, as-of date, audience, word count and canonical URL. METADATA ONLY: stu…`
- `query_knowledge_graph`: `The RELATIONS between the platform's teaching objects — which Academy module teaches which concept, which study covers which module, what a…`
- `search_concepts`: `Search the SAP AI & analytics concept encyclopaedia — the vocabulary of the stack, written for practitioners. Returns slug, title, category…`
- `search_firms`: `Search the published Analytics Legends directory of SAP AI & analytics service providers — placement agencies, Big-4 and ESN practices, SAP…`
- `search_news`: `Search the Analytics Legends market-news corpus. It is watched FOR SAP AI & analytics (Datasphere, Business Data Cloud, SAC, BW/4HANA, Data…`

## Changes

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
- 2026-09-09: [description changed](../../deltas/2026-09-09/44700875edd0c1c1f674.json): `2 field(s) changed`
- 2026-09-08: [description changed, schema changed](../../deltas/2026-09-08/44700875edd0c1c1f674.json): `9 field(s) changed; signals: length_more_than_doubled`
- 2026-09-05: [schema changed](../../deltas/2026-09-05/44700875edd0c1c1f674.json): `7 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://analyticslegends.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
