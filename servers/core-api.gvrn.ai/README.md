# core-api.gvrn.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/core-api.gvrn.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://core-api.gvrn.ai/incorporation-mcp` | 7 | [`c5cd88a3ba54`](28b1ca81d51b65e1728b.json) | 2026-08-29 |

## Tools at `https://core-api.gvrn.ai/incorporation-mcp`

- `create_incorporation_draft`: `Creates a new incorporation request draft bound to the verified email, using any fields provided. Requires a verificationToken from verify_…`
- `get_incorporation_guide`: `Returns the full GVRN incorporation workflow guide: the fields collected, the email-verification steps, and the review lifecycle. Also avai…`
- `get_incorporation_status`: `Returns the current status of an incorporation request (DRAFT → QUEUED_FOR_REVIEW → UNDER_REVIEW → COMPLETED). Requires a verificationToken…`
- `request_email_otp`: `Sends a 6-digit verification code to the given email address. The code is exchanged for a verificationToken via verify_email_otp, and that…`
- `submit_incorporation`: `Submits a draft for review by the GVRN team and returns the request status. Requires a verificationToken for the email that created the dra…`
- `update_incorporation_draft`: `Adds or corrects fields on an existing draft (patch semantics: only provided fields are changed; array fields are replaced whole). Requires…`
- `verify_email_otp`: `Verifies a 6-digit email code and returns a verificationToken valid for ~30 minutes. The draft tools require this token. Re-verifying the s…`

## Changes

- 2026-08-29: [annotation changed](../../deltas/2026-08-29/28b1ca81d51b65e1728b.json): `8 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://core-api.gvrn.ai/incorporation-mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
