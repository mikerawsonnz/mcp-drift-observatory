# agents-mcp.ironshard.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/agents-mcp.ironshard.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://agents-mcp.ironshard.ai/mcp` | 8 | [`281ea68e339e`](02ea3c2e611cb58662e1.json) | 2026-09-04 |

## Tools at `https://agents-mcp.ironshard.ai/mcp`

- `create_bucket`: `Creates a 30-day bucket and its secret bearer token.`
- `delete_object`: `Delete an object; versioned buckets may retain older versions.`
- `download_object`: `Return a secret, short-lived GET URL for an object's bytes.`
- `get_bucket`: `Return bucket details with storage and egress usage.`
- `get_bucket_permissions`: `Return currently permitted buckets and operations.`
- `get_object_metadata`: `Return an object's size, timestamps, ETag, content type, metadata, and tags.`
- `list_objects`: `List one page of objects and path-like prefixes, ordered by key.`
- `upload_object`: `Return a secret, short-lived PUT URL for an object up to 5 GB.`

## Changes

- 2026-09-04: [description changed, schema changed](../../deltas/2026-09-04/02ea3c2e611cb58662e1.json): `39 field(s) changed`
- 2026-08-27: [description changed, schema changed](../../deltas/2026-08-27/02ea3c2e611cb58662e1.json): `114 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://agents-mcp.ironshard.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
