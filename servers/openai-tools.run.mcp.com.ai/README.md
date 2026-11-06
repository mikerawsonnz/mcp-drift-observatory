# openai-tools.run.mcp.com.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/openai-tools.run.mcp.com.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://openai-tools.run.mcp.com.ai/mcp` | 9 | [`6bc3495876a0`](6bf156c00bfc2694eeef.json) | 2026-08-20 |

## Tools at `https://openai-tools.run.mcp.com.ai/mcp`

- `createImage`: `Creates an image given a prompt.`
- `createImageEdit`: `Creates an edited or extended image given an original image and a prompt.`
- `createImageVariation`: `Creates a variation of a given image.`
- `createModeration`: `Classifies if text violates OpenAI's Content Policy`
- `createTranscription`: `Transcribes audio into the input language.`
- `createTranslation`: `Translates audio into English.`
- `deleteModel`: `Delete a fine-tuned model. You must have the Owner role in your organization.`
- `listModels`: `Lists the currently available models, and provides basic information about each one such as the owner and availability.`
- `retrieveModel`: `Retrieves a model instance, providing basic information about the model such as the owner and permissioning.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://openai-tools.run.mcp.com.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
