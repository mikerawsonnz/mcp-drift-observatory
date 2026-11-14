# a2uicatalog.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/a2uicatalog.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://a2uicatalog.ai/mcp-docs` | 2 | [`40a8c2d85a07`](3c6cdbffd223af3533e0.json) | 2026-11-11 |
| `https://a2uicatalog.ai/mcp` | 40 | [`f1a2d63e9dd6`](57663a025cf9685e6622.json) | 2026-11-14 |

## Tools at `https://a2uicatalog.ai/mcp-docs`

- `list_docs`: `Use this to browse everything the documentation index holds when you have no specific query, or to see what topics exist before searching.…`
- `search_docs`: `Use this to answer a question about the product (auth, versioning, pricing, API surface, runbook catalog) from its own documentation, given…`

## Tools at `https://a2uicatalog.ai/mcp`

- `amiga`: `Open a real, cycle-exact Amiga 500 emulator in-chat (MCP Apps hosts only). Boots straight into AROS, a free open-source environment (no cop…`
- `build_multi_page_surface`: `Build a multi-section A2UI app from raw title+content sections — you never estimate size or decide how to split; each section becomes its o…`
- `deck_build`: `Build a PowerPoint (.pptx) file from a scene list or an A2UI payload. Deterministic (same input, same bytes), nothing is stored or fetched,…`
- `deck_schema`: `List the slide layouts the PPTX renderer builds (title, bullets, stats, quote, table, media, cta), each field with its limits, the targets,…`
- `deck_validate`: `Check a deck (scene list or A2UI payload) without building it. Returns every error with its slide, field and exact limit, warnings (no spea…`
- `delete_reading`: `Permanently remove one or more of the reader's saved readings from their History. Takes an array so the Workspace's multi-select can delete…`
- `describe_playbook`: `Explain a playbook to a HUMAN as a rendered surface: the frame it reads against, the lenses available, and the questions it will ask them.…`
- `diagram_studio`: `Draw a diagram in-chat with the full Diagram Studio interface (MCP Apps hosts only; it opens fullscreen where the host allows it). YOU writ…`
- `distill_document`: `Compile a training.md / roadmap markdown document into a live interactive A2UI app — DETERMINISTIC parser, no model involved. Fact sheet: i…`
- `drawio_open`: `Open a diagram you wrote in draw.io (diagrams.net). YOU write the diagram as mxGraph XML, the format draw.io reads; this tool checks it, an…`
- `emit_deployment`: `🎓 GRADUATE a tested surface into a dedicated, DEPLOYER-ONLY standing app in YOUR OWN Google Apps Script account. Returns a deterministic re…`
- `emit_runbook_surface`: `Stamp your content through a DECLARED runbook — a pre-authored, judgment-free surface composition. You supply content only; the runbook sup…`
- `emit_training_runbook`: `Build a multi-lesson training/course surface as ONE properly-linked page with real in-app tab navigation between lessons — prefer this over…`
- `export_reading`: `Export a kept reading as something that outlives this connector. format "html" returns ONE self-contained file — styles inlined, no network…`
- `find_atoms`: `Semantic search over the atom catalog: describe the UI piece you need in plain words and get the best-matching atoms, ranked best-first, ea…`
- `get_atom_schema`: `Return the PROP SHAPE (field names + what each field takes) for named atoms. get_catalog tells you an atom EXISTS; this tells you how to fi…`
- `get_catalog`: `Return one catalog's atoms (type + one-line description) so you know its vocabulary.`
- `get_profile`: `Read the signed-in reader's saved profile and recent history. Call this BEFORE asking a runbook's 'elicit' questions: if a domain or defaul…`
- `identify_model`: `CALL THIS FIRST, before any other a2ui-catalog tool, once per session. Declares your own model identity so this response can hand you capab…`
- `list_catalogs`: `List every A2UI catalog with a when-to-use, so you can pick the extension catalogs a surface needs. The base catalog (a2ui-atoms-v1) is alw…`
- `list_readings`: `The reader's recent stamped surfaces, newest first — what makes "compare this to my last three teardowns" answerable at all. Optionally fil…`
- `make_film`: `Make a short motion film (a social clip, launch teaser, quote card...) built by the A2UI Design Studio: you choose a template and supply th…`
- `make_surface_url`: `Render an A2UI payload in the CALLER'S OWN environment. Pass renderer_url (your deployed renderer /exec) and get a live URL + the catalogs…`
- `open_workspace`: `Open the A2UI Workspace — a rendered surface that IS the demo: each tool is introduced by the scenario it answers, then wired to run, then…`
- `preview_url`: `Quick DEMO render on the public renderer (ephemeral, nothing stored). Limited to 2 runs per client, then deploy your own renderer and use m…`
- `publish_url`: `STORES the payload server-side and returns a SHORT shareable link. Opt-in only: requires acknowledge_storage=true — confirm with the user f…`
- `read_article`: `Have the catalog's own model (Gemini) read an article through the article_playbook runbook and KEEP the reading in the signed-in reader's h…`
- `render_ping`: `Diagnostic: render a tiny test view in-chat (MCP Apps hosts only). Proves view mounting works independent of the full catalog renderer. Ech…`
- `render_reading_to_slack`: `Post a kept reading into Slack as real, native Block Kit — the continuity proof: generate here, save it, and the SAME content reopens in Sl…`
- `render_surface`: `Render an A2UI payload INSIDE the chat as a live interactive view (MCP Apps hosts only — on other hosts this returns the payload as text).…`
- `required_catalogs`: `Given an A2UI payload, return the resolvable catalog URIs it needs (deterministic — pure function of the atoms).`
- `save_profile`: `Update the signed-in reader's profile. Only the keys you pass change; pass null to clear one. Save what the reader TOLD you, never what you…`
- `save_reading`: `Record a stamped surface in the reader's history so it can be compared and reopened later. Call it AFTER emit_runbook_surface, and PASS ITS…`
- `sketch_agent_poll`: `Continue a sketch_agent_start task: returns every stroke newer than the given cursor (an event log, not a snapshot — nothing is skipped reg…`
- `sketch_agent_start`: `Start a real, live agent_sketchpad drawing: one Gemini call plans a complete picture as an ordered list of SVG strokes, the first stroke re…`
- `unlink_slack_account`: `Revoke one or more Slack accounts' link to this reader's store, from the Workspace side (the reverse of the Slack-side '/a2ui unlink' comma…`
- `unpublish_url`: `Delete a published short link before its TTL using the delete_token returned by publish_url.`
- `wall_calc`: `Compute a coursed block/brick wall specification — course and unit counts, weight, cost, mortar bags, a build-time curve across 1-6 builder…`
- `wasm_spike`: `Diagnostic (MCP Apps hosts only): mounts a view that instantiates a tiny hand-assembled WebAssembly module, computes per-frame state in it,…`
- `whoami`: `Report who this connection is authenticated as. Answers two SEPARATE questions that are easy to conflate: which APPLICATION is connected (t…`

## Changes

- 2026-11-14: [description changed, field changed, schema changed](../../deltas/2026-11-14/57663a025cf9685e6622.json): `25 field(s) changed; signals: length_more_than_doubled`
- 2026-11-12: [field changed](../../deltas/2026-11-12/57663a025cf9685e6622.json): `14 field(s) changed`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://a2uicatalog.ai/mcp-docs"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
