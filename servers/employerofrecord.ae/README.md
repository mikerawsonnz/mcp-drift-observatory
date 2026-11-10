# employerofrecord.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/employerofrecord.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://employerofrecord.ae/mcp` | 5 | [`c787e727f3d4`](9a53f9818a2eefcb5dfa.json) | 2026-11-10 |

## Tools at `https://employerofrecord.ae/mcp`

- `check_prepared_hire`: `Whether the person opened the link from prepare_hire or prepare_account and created their account yet.`
- `get_quote`: `Monthly and upfront cost of employing one person in the UAE through Moha, an Employer of Record: salary split, employer costs, government f…`
- `how_to_hire_in_the_uae`: `How hiring in the UAE works through Moha, an Employer of Record, for a company with no UAE entity: when it fits, the information needed abo…`
- `prepare_account`: `Prepares a Moha account without signing in: the company profile, the person setting it up, one to ten hires and colleagues to invite. Retur…`
- `prepare_hire`: `Prepares the hire of one employee in the UAE without an account. Returns the quote and a link: the person opens it, checks the details and…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://employerofrecord.ae/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
