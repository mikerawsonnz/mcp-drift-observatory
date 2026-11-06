# drift.getvda.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/drift.getvda.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://drift.getvda.ai/mcp` | 6 | [`74daec8d08ac`](b7e55bf8230ad605a287.json) | 2026-08-21 |

## Tools at `https://drift.getvda.ai/mcp`

- `drift_check`: `FREE. Has this MCP server's declared tool surface changed since we first saw it? Returns the current hash, when it last changed, how many t…`
- `drift_diff`: `What actually changed: field-level detail for this server's observed changes, including which tool moved and whether the change touched a d…`
- `drift_hash`: `FREE. Canonically hash a tool list you supply, so you can confirm your implementation reproduces our bytes before trusting any hash we publ…`
- `drift_probe`: `Fetch this server RIGHT NOW and compare it to our stored baseline. Use when you need a fresh answer rather than the last scheduled observat…`
- `drift_status`: `FREE. Coverage of the MCP Drift Observatory: how many public MCP servers we have discovered, how many we can actually observe, and how many…`
- `selftest`: `FREE, no payment required. Runs this agent's real capability on a fixed canned input and returns the genuine result, an honest assertion gr…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://drift.getvda.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
