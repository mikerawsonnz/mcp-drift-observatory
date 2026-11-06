# dataecho.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/dataecho.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://dataecho.ai/mcp` | 26 | [`4807c875821c`](afe43c5bab2c6b69cdd2.json) | 2026-08-20 |

## Tools at `https://dataecho.ai/mcp`

- `app_status`: `Build/run status of a container app deployed via publish_site with a Dockerfile. Poll until status is 'live' or 'failed'.`
- `claim_site`: `Make a previously-anonymous site permanent under the authenticated account (requires auth + the claimToken from publish_site).`
- `create_drive`: `Create a new private drive.`
- `delete_site`: `Permanently delete an owned site. Irreversible — confirm with the user first.`
- `delete_variable`: `Delete an account variable.`
- `drive_delete_file`: `Delete one file from a drive.`
- `drive_history`: `Version timeline of a drive (every write is a restorable version).`
- `drive_list_files`: `List files in a drive (by drive name or drv_… id), optionally under a path prefix.`
- `drive_move_file`: `Move/rename a file inside a drive.`
- `drive_read_file`: `Read a file from a drive. Text comes back as utf-8 'content'; binary as 'contentBase64'. Files over 1 MB are refused (use the skill scripts…`
- `drive_restore`: `Restore a drive to a prior version (commits a new version; nothing is lost).`
- `drive_revoke_token`: `Revoke a drive share token.`
- `drive_share`: `Mint a scoped drive access token for another agent (perms read/write, optional path prefix + TTL like '7d'). The secret is returned ONCE.`
- `drive_tokens`: `List active share tokens of a drive (secrets are never shown again).`
- `drive_write_file`: `Write/overwrite one file in a drive (ETag-safe: pass ifMatch to assert the version you read, otherwise the current version is used automati…`
- `get_site`: `Full details + current file manifest of an owned site.`
- `list_drives`: `List the authenticated account's private cloud drives.`
- `list_sites`: `List all sites owned by the authenticated account.`
- `list_variables`: `List account variable NAMES (values are write-only — they are injected into proxy calls and container apps, never read back).`
- `platform_info`: `DataEcho platform overview: what it can host, auth state of this connection, docs links. Call this first if unsure.`
- `publish_site`: `Deploy files to a live URL. No slug → create a NEW site (works without auth; anonymous sites expire in 24h — always show the user the claim…`
- `request_login_code`: `Start sign-in: email a one-time code to the user. Follow with verify_login_code.`
- `search_sites`: `Full-text search across the authenticated account's sites (names, metadata, and text content).`
- `set_variable`: `Create/update a write-only account secret (uppercase name). Injected as env vars into container apps and as ${VAR} into proxy calls. Option…`
- `update_site_metadata`: `Patch site settings without redeploying: viewer title/description, SPA mode, TTL, password (string sets, null removes).`
- `verify_login_code`: `Complete sign-in with the emailed code. Returns the apiKey ONCE — configure it as the 'Authorization: Bearer <key>' header of this MCP conn…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://dataecho.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
