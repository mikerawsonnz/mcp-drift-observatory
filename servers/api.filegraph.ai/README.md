# api.filegraph.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.filegraph.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.filegraph.ai/mcp` | 9 | [`f206c39e106f`](030f8d70b17734691deb.json) | 2026-09-15 |

## Tools at `https://api.filegraph.ai/mcp`

- `filegraph_api_overview`: `API overview: authentication, rate limits, errors, and available endpoint groups.`
- `filegraph_html_processing_docs`: `Docs for /html/to-text, /html/to-pdf, /html/to-image — extract html text, render to pdf, capture html screenshots.`
- `filegraph_image_processing_docs`: `Docs for /image/to-text, /image/to-pdf, /image/resize — extract text via ocr, convert images to pdf, resize images.`
- `filegraph_office_documents_docs`: `Docs for /docx/to-text, /docx/to-pdf, /xlsx/to-text, /xlsx/to-pdf, /xlsx/to-csv, /pptx/to-text, /pptx/to-pdf, /pptx/to-images — extract tex…`
- `filegraph_pdf_manipulation_docs`: `Docs for /pdf/merge, /pdf/split, /pdf/compress, /pdf/rotate — merge, split, compress, and rotate pdf files.`
- `filegraph_pdf_security_docs`: `Docs for /pdf/encrypt, /pdf/decrypt — encrypt and decrypt pdf files with password protection.`
- `filegraph_pdf_text_conversion_docs`: `Docs for /pdf/to-text, /pdf/to-docx, /pdf/to-image — extract text with ocr, convert pdf to docx or images.`
- `filegraph_security_docs`: `Docs for /security/pdf/redact, /security/text/redact, /security/pdf/lock, /security/pdf/unlock, /security/detect-tracking — redact sensitiv…`
- `filegraph_text_extraction_docs`: `Docs for /any/to-text, /any/info, /any/to-struct — extract text with smart format detection and ocr, analyze file metadata, extract structu…`

## Changes

- 2026-09-15: [field changed](../../deltas/2026-09-15/030f8d70b17734691deb.json): `9 field(s) changed`
- 2026-09-04: [field changed](../../deltas/2026-09-04/030f8d70b17734691deb.json): `18 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.filegraph.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
