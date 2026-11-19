# drift.getvda.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/drift.getvda.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://drift.getvda.ai/mcp` | 6 | [`d87d025f0bf5`](b7e55bf8230ad605a287.json) | 2026-11-19 |

## Tools at `https://drift.getvda.ai/mcp`

- `drift_check`: `Has this MCP server's declared tool surface changed since we first saw it? Returns the current hash, when it last changed, how many times,…`
- `drift_diff`: `What actually changed: field-level detail for this server's observed changes, including which tool moved and whether the change touched a d…`
- `drift_hash`: `Canonically hash a tool list you supply, so you can confirm your implementation reproduces our bytes before trusting any hash we publish. e…`
- `drift_probe`: `Fetch this server right now and compare it to our stored baseline. Use when you need a fresh answer rather than the last scheduled observat…`
- `drift_status`: `Coverage of the MCP Drift Observatory: how many public MCP servers we have discovered, how many we can actually observe, and how many are a…`
- `selftest`: `Free, no payment required. Runs this agent's real capability on a fixed canned input and returns the genuine result, an honest assertion gr…`

## Changes

- 2026-11-19: [annotation changed, description changed, field changed](../../deltas/2026-11-19/b7e55bf8230ad605a287.json): `41 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://drift.getvda.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
