# duskly.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/duskly.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://duskly.ai/mcp` | 10 | [`7422e6b5072a`](c0b3659ee2439b75ae37.json) | 2026-09-26 |

## Tools at `https://duskly.ai/mcp`

- `duskly_classify_edit`: `Whether a given edit to a real estate listing photo must be disclosed, and whether any market prohibits it outright. Use this before tellin…`
- `duskly_generate_disclosure`: `The exact disclosure text to publish alongside an edited listing photo, written for each surface it has to appear on: the MLS photo descrip…`
- `duskly_get_checkout_url`: `A Stripe Checkout URL for an unpaid listing, for a **person** to open and pay. Duskly does not take payment through MCP and no agent comple…`
- `duskly_get_listing`: `The state of a Duskly listing: how many photos it holds, which have been edited, whether it has been paid for, and how much of its render b…`
- `duskly_get_listing_pack`: `Everything a paid listing returns: the download link for the archive, the disclosure wording for every edited photo, and the public page sh…`
- `duskly_get_pricing`: `Duskly's price and what a paid listing returns. Use this when someone asks what it costs or what they get. Editing is not available over MC…`
- `duskly_list_edits`: `Every edit Duskly performs, with what it does and how it is classified for disclosure. Use this to pick the right edit for what someone is…`
- `duskly_list_prohibited_alterations`: `Edits that are prohibited outright in one or more markets and are never made acceptable by adding a disclosure. Use this when someone asks…`
- `duskly_start_listing`: `Returns the URL a person should open to upload listing photos and run an edit themselves. Use this when someone wants an edit performed. Ed…`
- `duskly_verify_image`: `Inspect an image for provenance signals: an invisible Duskly watermark, IPTC digital source type metadata, and whether a C2PA container app…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://duskly.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
