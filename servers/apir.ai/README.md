# apir.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/apir.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://apir.ai/api/mcp` | 3 | [`7340e3b3b3bf`](28b58debdb73ae5a9b8c.json) | 2026-11-09 |

## Tools at `https://apir.ai/api/mcp`

- `check_authority`: `Resolve the human mandate behind an AI agent: which actions a named person actually permitted, any value cap, the expiry, and whether the g…`
- `get_verification_keys`: `Return the Ed25519 public keys APIR publishes, so a signature can be recomputed offline without trusting any APIR response, including this…`
- `verify_agent`: `Check whether an AI agent carries a real, cryptographically signed credential. Accepts an agent name, a credential id (TP-...), an agent UU…`

## Changes

- 2026-11-09: [annotation changed](../../deltas/2026-11-09/28b58debdb73ae5a9b8c.json): `15 field(s) changed`
- 2026-10-31: [description changed](../../deltas/2026-10-31/28b58debdb73ae5a9b8c.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://apir.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
