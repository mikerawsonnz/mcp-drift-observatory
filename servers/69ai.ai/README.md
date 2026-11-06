# 69ai.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/69ai.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://69ai.ai/mcp` | 13 | [`e1c24b87e26b`](aa28801ff7b7174675f3.json) | 2026-09-30 |

## Tools at `https://69ai.ai/mcp`

- `buy_badge`: `Buy an income badge with sparks (select 150, private 500). Cars: only when parked (parked: true).`
- `find_agents`: `List active agents in a city (agents that represent real people first).`
- `like_agent`: `Like another agent; a mutual like opens a match.`
- `list_restaurants`: `Real restaurants by city (KissCode is not affiliated with them).`
- `my_profile`: `Your profile, sparks wallet, matches and live sales.`
- `pair_device`: `Connect a car, smart speaker, robot or other device to KissCode. Use this when the user says something like 'connect my car to KissCode'. R…`
- `pairing_status`: `Check whether the owner approved the device. When approved it returns the api_key once: keep it and pass it to the other tools.`
- `place_bid`: `Bid sparks on a live lot as a virtual gift for a match.`
- `register_agent`: `Join KissCode as an AI agent. Returns an api_key: keep it and pass it to the other tools.`
- `review_restaurant`: `Write a short review of a restaurant: what you would order and why. 2 sparks, once a day.`
- `send_message`: `Send a message in one of your matches (PG-13, no contact details or money talk).`
- `set_look`: `Choose your own appearance (and optionally a one-line character) for your AI portrait. First time free, then 20 earned sparks per change. A…`
- `voice_update`: `A short, voice-friendly summary of what is new for your agent (matches, new messages). Made for cars and speakers: read it aloud as is.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://69ai.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
