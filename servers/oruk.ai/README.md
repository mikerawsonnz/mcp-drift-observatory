# oruk.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/oruk.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://oruk.ai/mcp` | 7 | [`d9de487d7e2d`](0ec2fb8e500cb4b4b194.json) | 2026-08-20 |

## Tools at `https://oruk.ai/mcp`

- `oruk_analyze_speech`: `Transcribe English audio AND score how it was said in one call: transcript, tagged transcript, calibrated emotion (15 labels) and speaking-…`
- `oruk_analyze_tone`: `Score how speech sounds without transcribing it: calibrated multilabel emotion (happy, frustrated, worried, …) and speaking-style (sarcasti…`
- `oruk_check_credits`: `Verify that an oruk API key works and report the organization’s plan, remaining credit balance, and recent API usage. Use this as the first…`
- `oruk_create_trial_key`: `Mint a real, temporary oruk API key with no account required: 3 requests, expires in 30 minutes, spends from a capped shared budget. Use th…`
- `oruk_get_started`: `Quickstart for the oruk Speech API and this MCP server: how to get an API key, per-client MCP configuration snippets, SDK install commands,…`
- `oruk_list_models`: `List oruk’s speech models with lifecycle and per-task pricing (USD per audio minute), the five API tasks, the 15 emotion and 16 speaking-st…`
- `oruk_transcribe_audio`: `Transcribe prerecorded English audio to text with time-ordered segments and word timings. Use this when only the words matter. Accepts a pu…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://oruk.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
