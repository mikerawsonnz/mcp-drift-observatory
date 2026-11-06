# datephotos.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/datephotos.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://datephotos.ai/api/mcp` | 3 | [`07c01c42c88f`](111c6a461ad65881b716.json) | 2026-10-15 |

## Tools at `https://datephotos.ai/api/mcp`

- `audit_dating_photo`: `Score one dating-profile photo 0-100 and list concrete issues and fixes (lighting, framing, face visibility, background, realism). Takes a…`
- `check_ai_photo_policy`: `Whether Tinder, Hinge and Bumble allow AI-generated or AI-edited profile photos, how they detect them, what happens if you break the rules,…`
- `get_dating_app_photo_rules`: `Official photo rules for a dating app (Tinder, Hinge or Bumble): how many photos, how verification works, what is not allowed, and its AI-p…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://datephotos.ai/api/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
