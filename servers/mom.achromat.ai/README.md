# mom.achromat.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mom.achromat.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mom.achromat.ai/mcp` | 1 | [`99aaf83d7a4d`](b8f5252d1461a57e0368.json) | 2026-11-22 |

## Tools at `https://mom.achromat.ai/mcp`

- `achromat_recall`: `SANDBOX PREVIEW of Achromat Machine Operational Memory. It takes the same input as the full achromat_recall, but this public endpoint does…`

## Changes

- 2026-11-22: [schema changed](../../deltas/2026-11-22/b8f5252d1461a57e0368.json): `4 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mom.achromat.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
