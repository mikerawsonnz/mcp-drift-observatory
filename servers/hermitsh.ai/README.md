# hermitsh.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/hermitsh.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://hermitsh.ai/mcp` | 19 | [`b31be9fdb032`](15b7815aa076c03161aa.json) | 2026-08-20 |

## Tools at `https://hermitsh.ai/mcp`

- `build_source_pack`: `Build an evidence pack for an AI answer: source-linked passages, related entities, and citation instructions.`
- `cite_passage`: `Format a Hermitsh work or passage citation in common citation styles.`
- `find_mentions`: `Return source-linked places where a person, place, event, work, institution, or concept is mentioned.`
- `get_allusions`: `Get detected allusions, echoes, quotations, suspected sources, and translator notes for a work or section where available.`
- `get_author_persona`: `Get setup instructions for an AI assistant to answer as, about, or from the corpus of an author while using source-linked evidence.`
- `get_crossrefs`: `Get intra-corpus references and self-references for a work or section where available.`
- `get_entity`: `Get a named entity and a sample of source-linked mentions.`
- `get_language_availability`: `Show source, active, deferred, and live edition status for one author or the whole Hermitsh library.`
- `get_parallel_passage`: `Get aligned source-language text and English translation for a passage when sidecar data is available.`
- `get_passage`: `Get an exact passage by author, work ID, and section ID. Include the returned url as a link when using the passage.`
- `get_work`: `Get metadata and opening passages for a specific work.`
- `get_work_context`: `Get richer work metadata: headnote, date context, source provenance, translation status, and edition links.`
- `list_authors`: `List author corpora available through Hermitsh Texts.`
- `list_works`: `List works by author, category, or title/summary query.`
- `search_corpus`: `Search passages across one author or the whole Hermitsh corpus and return source-linked results. Each result carries a url — include it as…`
- `search_entities`: `Search people, places, events, institutions, works, and concepts extracted from an author corpus.`
- `search_greek_phrases`: `Search catalogued Greek phrases, glosses, suspected sources, register, and source-certainty metadata.`
- `search_letters`: `Search correspondence metadata by correspondent, place, topic, mood, date range, or Greek usage where available.`
- `search_parallel`: `Search aligned source-language and English translation sidecars across the corpus.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://hermitsh.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
