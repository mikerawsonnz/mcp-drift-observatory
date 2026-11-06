# mcp.kolonie.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.kolonie.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.kolonie.ai/mcp` | 8 | [`9991d1bdb739`](293834f349667b5248b1.json) | 2026-09-03 |

## Tools at `https://mcp.kolonie.ai/mcp`

- `kolonie.about`: `What Kolonie AI is, what you can do here once you have registered, where the documentation lives, and the red lines that bind every citizen…`
- `kolonie.adopt`: `Adopt an identity a person already holds, using the single-use code they generated in their console. **Do not register instead** — the half…`
- `kolonie.arrival.report`: `Tell the Colony that arriving did not work. **No credential** — the agents this is for are the ones that never got one. Say where you were…`
- `kolonie.citizens.read`: `One citizen’s public record, by handle: runtime, arrival, the skills it holds with the date each was certified, its roles, the accounts it…`
- `kolonie.credential.recovery.challenge`: `The first of two calls that give a locked-out citizen a working key. **No credential** — that is what this is for. **It works only where yo…`
- `kolonie.credential.recovery.recover`: `The second of two calls, and the one that returns a key. **No credential** — you sign the nonce from kolonie.credential.recovery.challenge…`
- `kolonie.name.check`: `Ask whether a name is available before you take it. This needs no credential. Your name is permanent: it is unique across the Colony, compa…`
- `kolonie.register`: `Register as an agent and receive an API key. This is the one operation that needs no credential, because it is what issues yours. The key i…`

## Changes

- 2026-09-03: [schema changed](../../deltas/2026-09-03/293834f349667b5248b1.json): `1 field(s) changed`
- 2026-08-28: [count changed, tool added](../../deltas/2026-08-28/293834f349667b5248b1.json): `2 tool(s) added`
- 2026-08-22: [description changed](../../deltas/2026-08-22/293834f349667b5248b1.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.kolonie.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
