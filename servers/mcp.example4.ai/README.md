# mcp.example4.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.example4.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.example4.ai/mcp` | 16 | [`1f233ec90ec1`](b8a81b4fe9c2f281582e.json) | 2026-08-20 |

## Tools at `https://mcp.example4.ai/mcp`

- `xmp4_callees`: `Find direct callees (methods called by) a symbol in a project. Navigate step-by-step by calling xmp4_callees again on interesting results.`
- `xmp4_callers`: `Find direct callers of a symbol in a project. Navigate step-by-step by calling xmp4_callers again on interesting results.`
- `xmp4_deps`: `List external dependencies of a project.`
- `xmp4_grep`: `Server-side regex text search over indexed project source files. Free tier: requires file_path (single file). Premium tier (XMP4_PREMIUM_GR…`
- `xmp4_guide`: `Usage guide for xmp4 tools — read this first to learn the correct workflow`
- `xmp4_hierarchy`: `Get type hierarchy (base, interfaces, derived) for a symbol in a project.`
- `xmp4_info`: `Get detailed information about a symbol in a project.`
- `xmp4_outline`: `Get outline (all symbols) for a file in a project.`
- `xmp4_projects`: `Search and browse projects by language and name. Use this first to discover projects, then use other tools with the repo name.`
- `xmp4_search`: `Search symbols in a project. Use xmp4_projects first to find the project identifier.`
- `xmp4_server`: `Get server information, version, and capabilities`
- `xmp4_source`: `Extract source code for a symbol in a project.`
- `xmp4_symbol_at`: `LSP-style position→symbol lookup. Given (file_path, line, column) returns the symbol whose occurrence covers that cursor position. line is…`
- `xmp4_tests_for`: `Find direct tests that exercise a given symbol (direct callers filtered to test-file candidates per language pattern: CSharp/Java/PHP: *Tes…`
- `xmp4_usages`: `Find all usages/references of a symbol in a project.`
- `xmp4_view`: `Read a raw file excerpt from an indexed project by line range. Use after xmp4_search/xmp4_outline locates the region of interest, or to exp…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.example4.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
