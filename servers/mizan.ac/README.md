# mizan.ac: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mizan.ac.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mizan.ac/mcp` | 5 | [`8ab082461ef2`](70c77423ed2d6ce6e69e.json) | 2026-11-10 |

## Tools at `https://mizan.ac/mcp`

- `check_players`: `Check up to 100 Steam accounts in one call, such as everyone on a game server: each account's bans across every list Mizan reads, whether a…`
- `list_my_communities`: `List the communities you belong to on Mizan, your role in each, their registry status and their game servers. Needs you to sign in to Mizan.`
- `list_sources`: `List the ban lists Mizan reads, largest first: each list's name, who issues its bans, the games it covers, its bans and how many are in for…`
- `lookup_player`: `Look up a player's Mizan record: their bans across every list Mizan reads, whether any list banned them for cheating, and Steam's own VAC a…`
- `registry_stats`: `The size of Mizan's registry: how many ban lists it reads, the bans on them, how many are in force, and the same counts for each game.`

## Changes

- 2026-11-10: [schema changed](../../deltas/2026-11-10/70c77423ed2d6ce6e69e.json): `5 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mizan.ac/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
