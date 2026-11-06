# aient.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/aient.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://aient.ai/mcp` | 2 | [`abf25e7155f2`](7e1a6afbaa08fbb9992b.json) | 2026-09-18 |

## Tools at `https://aient.ai/mcp`

- `signup`: `Create an Aient account from an email address, or get a sign-in code for an existing one, with no browser and no token. **When to use**: yo…`
- `verify_email`: `Confirm the code Aient emailed after 'signup' and receive the access token for this MCP server. **Returns**: 'access_token' (a Bearer token…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://aient.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
