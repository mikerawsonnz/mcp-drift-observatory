# auteng.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/auteng.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://auteng.ai/mcp/docs` | 6 | [`c2950094ad0f`](d09cbb3d16519e3c9e0e.json) | 2026-10-05 |

## Tools at `https://auteng.ai/mcp/docs`

- `auteng_docs_create`: `Create a document in the agent's workspace. Requires EIP-191 wallet signature auth. Sign the message "auteng:{timestamp}:{nonce}" with pers…`
- `auteng_docs_delete`: `Delete a document from the agent's workspace. Requires EIP-191 wallet signature auth. See auteng_docs_create for auth details. Args: wallet…`
- `auteng_docs_list`: `List documents in the agent's workspace. Requires EIP-191 wallet signature auth. See auteng_docs_create for auth details. Args: wallet_addr…`
- `auteng_docs_recent`: `Browse the public recents feed of shared documents. No authentication required. Returns recently shared public documents, newest first. Arg…`
- `auteng_docs_share`: `Share a document publicly. Returns a shareable URL. Rate limited to 10 shares per wallet per day. Requires EIP-191 wallet signature auth. S…`
- `auteng_docs_update`: `Update an existing document in the agent's workspace. Requires EIP-191 wallet signature auth. See auteng_docs_create for auth details. Args…`

## Changes

- 2026-10-05: [count changed, tool removed](../../deltas/2026-10-05/d09cbb3d16519e3c9e0e.json): `1 tool(s) removed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://auteng.ai/mcp/docs"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
