# api.powerline.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.powerline.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.powerline.ai/v1/mcp` | 4 | [`39ca8e457baa`](ab0c319ca0258394a94c.json) | 2026-08-20 |

## Tools at `https://api.powerline.ai/v1/mcp`

- `get_job`: `Get the status and screenshots for a preview job. Poll until status is "completed".`
- `get_screenshot`: `Fetch a rendered screenshot. Returns the image URL for the given job, client, width, and environment (color scheme / images).`
- `list_clients`: `List the email clients this deployment can render right now, with their rendering tier, engine, and capabilities`
- `submit_preview`: `Submit an email for rendering across email clients — full HTML, or a complete raw .eml (base64). Provide exactly one of html/eml. Returns a…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.powerline.ai/v1/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
