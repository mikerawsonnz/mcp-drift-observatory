# linkedin.run.mcp.com.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/linkedin.run.mcp.com.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://linkedin.run.mcp.com.ai/mcp` | 3 | [`8bfc73ecc215`](30817f826a5b2e4bdb90.json) | 2026-08-20 |

## Tools at `https://linkedin.run.mcp.com.ai/mcp`

- `createSharePost`: `Share on LinkedIn, create a share post - Create a new share post on LinkedIn using text, URLs, and images`
- `getPersonProfile`: `Get person profile - Get basic profile information for a person`
- `getSharePosts`: `Get share posts - Retrieve share posts for the authenticated user or organization`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://linkedin.run.mcp.com.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
