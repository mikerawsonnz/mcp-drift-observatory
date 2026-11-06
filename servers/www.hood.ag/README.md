# www.hood.ag: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.hood.ag.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.hood.ag/api/mcp` | 5 | [`3b8f4feacba4`](d321fce0eb562987695e.json) | 2026-09-04 |

## Tools at `https://www.hood.ag/api/mcp`

- `check_availability`: `Check whether a .hood name is available to register, and its yearly price.`
- `name_info`: `Full snapshot of a .hood name: resolved address, NFT owner, expiry, and availability.`
- `resolve_name`: `Forward-resolve a .hood name to the address it points to. Returns null if unset.`
- `resolve_text`: `Read a text record (e.g. "avatar", "url", "com.twitter") set on a .hood name.`
- `reverse_resolve`: `Reverse-resolve an address to its primary .hood name. 'verified' is true only when the name's forward record points back to the address.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.hood.ag/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
