# app.mindola.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/app.mindola.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://app.mindola.ai/mcp/lens` | 3 | [`810e08cd011b`](c7fbe9817143c0cc4895.json) | 2026-08-20 |

## Tools at `https://app.mindola.ai/mcp/lens`

- `add_lens_knowledge`: `Add text notes or URLs to a Mindola lens created in this conversation (before it is claimed). Content runs through the standard ingest pipe…`
- `create_digital_twin_lens`: `Create a shareable Mindola lens (AI clone) from a profile the user has approved in this conversation. Call this only after summarizing the…`
- `get_lens_status`: `Check a Mindola lens: its share URL, whether it has been claimed, and how much of its knowledge has finished ingesting (ready / pending / f…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://app.mindola.ai/mcp/lens"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
