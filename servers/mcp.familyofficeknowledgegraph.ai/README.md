# mcp.familyofficeknowledgegraph.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.familyofficeknowledgegraph.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.familyofficeknowledgegraph.ai/mcp` | 5 | [`db45fbe5221f`](beab443619af2b5039ee.json) | 2026-09-18 |

## Tools at `https://mcp.familyofficeknowledgegraph.ai/mcp`

- `get_record`: `The Family Office Record for one identifier: every field with value, source_url, read_by and state; optionally a named version.`
- `list_aliases`: `Every name the record carries for one identifier — legal name, register names, other names — each with its source.`
- `list_events_since`: `Dated, URL'd events on one record (registrations, renewals, orders, acquisitions), oldest first, optionally since a date, paged by cursor.`
- `list_nodes`: `The graph's nodes — one per jurisdiction — with record counts read from each node's index, the node door and its as-of.`
- `resolve_family_office`: `Resolve an identifier (LEI, legal name, alias or register id) to the family-office records that carry it, with the node that serves each.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.familyofficeknowledgegraph.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
