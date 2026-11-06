# deepdna.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/deepdna.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://deepdna.ai/mcp` | 6 | [`ecdd8fb26c01`](e890009185db847fd4ca.json) | 2026-10-12 |

## Tools at `https://deepdna.ai/mcp`

- `check_medications`: `Given a list of generic drug names, say which ones have a curated drug–gene record, with which genes and what each record rests on (a CPIC…`
- `list_genes`: `List the genes in the DeepDNA knowledge base, with a one-line summary and category for each.`
- `lookup_drug_gene`: `Pharmacogenomic guidance for a gene, optionally for one drug: guideline (CPIC or DPWG, "drug label", or null when the record rests on the p…`
- `lookup_gene`: `Everything curated about one gene: function, key variants with rsIDs, metabolizer or function phenotypes, drug interactions, what a consume…`
- `lookup_variant`: `One variant by dbSNP rsID: gene, star-allele or common name, alleles, functional effect, population frequency and sources. Optionally pass…`
- `request_beta_access`: `Register the user's interest in DeepDNA's private beta (DNA file parsing, annotation, bloodwork; not deployed yet). Only call this after th…`

## Changes

- 2026-10-12: [count changed, description changed, schema changed, tool added](../../deltas/2026-10-12/e890009185db847fd4ca.json): `2 tool(s) added; 4 field(s) changed; signals: length_more_than_doubled, url_introduced`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://deepdna.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
