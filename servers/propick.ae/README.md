# propick.ae: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/propick.ae.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://propick.ae/mcp` | 8 | [`87efc210c90f`](91748b15f7242e1c689f.json) | 2026-08-26 |

## Tools at `https://propick.ae/mcp`

- `get_reference`: `Every closed vocabulary and limit of the import payload in one call: categories, listing types, building statuses, rental periods, occupanc…`
- `get_run`: `Fetch one import run by importId: status, counters of planned and applied decisions, stop reason if the run did not finish.`
- `list_events`: `Per-property outcomes of import runs: what happened to each externalPropertyId, with error codes and details. Filter by importId and/or ext…`
- `list_responsibles`: `List agency members that can be set as responsibleUsername on a listing. Agency channels only: a personal channel gets a refusal, not an em…`
- `list_runs`: `List this channel import runs, newest first. Paginated.`
- `ping`: `Health check for the integration key. Returns the channel clientId. Call once after connecting to verify the key works.`
- `search_projects`: `Resolve a development project to the numeric projectId required by every listing in sync_properties. Search by name fragment (min 2 charact…`
- `sync_properties`: `Submit a batch of property listings (up to 500) for import. The engine diffs the batch against the channel current stock and plans creation…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://propick.ae/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
