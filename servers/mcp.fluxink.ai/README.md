# mcp.fluxink.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.fluxink.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.fluxink.ai/servers/f6b6758dba6c4c92b83407a113fdb80b/mcp` | 6 | [`d7e1a0270636`](dad03afd7680df29887a.json) | 2026-08-20 |

## Tools at `https://mcp.fluxink.ai/servers/f6b6758dba6c4c92b83407a113fdb80b/mcp`

- `fluxink-mcp-chatgpt-create-layout`: `FluxInk document layout generator. Transform raw text content into a structured PDF using one of seven study or work templates, then previe…`
- `fluxink-mcp-chatgpt-recognize-handwriting`: `Internal FluxInk handwriting recognition execution endpoint. Invoked ONLY by the handwriting canvas widget when the user finishes drawing.…`
- `fluxink-mcp-chatgpt-recognize-image`: `FluxInk image text recognition. Extract text from an EXISTING image (file upload, URL, or base64) the user provides. Higher accuracy than b…`
- `fluxink-mcp-chatgpt-show-handwriting-canvas`: `Open the FluxInk handwriting recognition canvas. The user draws freehand strokes with a stylus, finger, or mouse. The strokes are converted…`
- `fluxink-mcp-chatgpt-show-style-canvas`: `Open the FluxInk natural texture ink style capture canvas. The user draws a few sample characters in a personal handwriting style. The widg…`
- `fluxink-mcp-chatgpt-synthesize-handwriting-style`: `Internal FluxInk natural texture ink execution endpoint. Invoked ONLY by the style canvas widget when the user clicks Generate. Do NOT call…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.fluxink.ai/servers/f6b6758dba6c4c92b83407a113fdb80b/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
