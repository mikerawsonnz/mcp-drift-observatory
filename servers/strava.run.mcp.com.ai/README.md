# strava.run.mcp.com.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/strava.run.mcp.com.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://strava.run.mcp.com.ai/mcp` | 13 | [`e1ac7517d5ad`](0cb77392382df51bfbf7.json) | 2026-08-24 |

## Tools at `https://strava.run.mcp.com.ai/mcp`

- `exploreSegments`: `Explore segments - Returns the top 10 segments matching a specified query.`
- `getClubActivitiesById`: `List Club Activities - Retrieve recent activities from members of a specific club. The authenticated athlete must belong to the requested c…`
- `getClubAdminsById`: `List Club Administrators - Returns a list of the administrators of a given club.`
- `getClubById`: `Get Club - Returns a given club using its identifier.`
- `getClubMembersById`: `List Club Members - Returns a list of the athletes who are members of a given club.`
- `getEffortsBySegmentId`: `List Segment Efforts - Returns a set of the authenticated athlete's segment efforts for a given segment. Requires subscription.`
- `getGearById`: `Get Equipment - Returns an equipment using its identifier.`
- `getLoggedInAthlete`: `Get Authenticated Athlete - Returns the currently authenticated athlete. Tokens with profile:read_all scope will receive a detailed athlete…`
- `getLoggedInAthleteClubs`: `List Athlete Clubs - Returns a list of the clubs whose membership includes the authenticated athlete.`
- `getLoggedInAthleteStarredSegments`: `List Starred Segments - List of the authenticated athlete's starred segments. Private segments are filtered out unless requested by a token…`
- `getRoutesByAthleteId`: `List Athlete Routes - Returns a list of the routes created by the authenticated athlete. Private routes are filtered out unless requested b…`
- `getSegmentEffortById`: `Get Segment Effort - Returns a segment effort from an activity that is owned by the authenticated athlete. Requires subscription.`
- `getStats`: `Get Athlete Stats - Returns the activity stats of an athlete. Only includes data from activities set to Everyone visibility.`

## Changes

- 2026-08-24: [description changed](../../deltas/2026-08-24/0cb77392382df51bfbf7.json): `1 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://strava.run.mcp.com.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
