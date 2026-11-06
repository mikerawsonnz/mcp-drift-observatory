# api.cueframe.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/api.cueframe.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://api.cueframe.ai/v1/mcp` | 72 | [`20b71de41a5a`](b25e350a1ddb55a63705.json) | 2026-10-16 |

## Tools at `https://api.cueframe.ai/v1/mcp`

- `apply_composition`: `Atomically apply an array of CompositionOps to a project composition. All ops succeed or none do (transactional). Call describe_composition…`
- `apply_template`: `Insert a resolved builtin component package into an existing project. Pass template as the selected builtin id and body with projectId, the…`
- `cancel_compose`: `Cancel an in-flight compose job (stop a runaway/mis-priced ensemble). Needs projectId + composeJobId (from compose). The director cancel is…`
- `cancel_export`: `Cancel an in-flight NLE export (fcpxml/premiere). Needs projectId + exportId (from the export enqueue). No-op-reject (422) if already termi…`
- `cancel_job`: `Cancel a running async job (verify / preview / brand-kit-extract) returned by an enqueue call — abort a mis-priced job instead of waiting o…`
- `cancel_render`: `Cancel an in-flight render (stop a runaway/queued job). Needs projectId + renderId (from create_render). No-op if already terminal.`
- `compose`: `Start an async Director compose job: it authors an ensemble of full composition candidates, verifies each, and saves the winner to the proj…`
- `consult`: `Ask the Director for editing advice on the project's CURRENT composition — it NEVER writes your composition (you stay the decider). Async:…`
- `create_brand_kit`: `Create or UPSERT a brand kit (re-POSTing the same kitId updates it in place — this is also the brand-kit UPDATE path). Sets fonts/colors/lo…`
- `create_brief`: `Persist the video's INTENT as a Brief — the Director's rich input contract (spec: the storyboard skill's output lands here). Fields: goal (…`
- `create_checkout`: `Top up the CURRENT org's credit wallet. Body { plan: "credit_pack_10"/"credit_pack_30"/"credit_pack_100" } → returns { url }: a hosted Stri…`
- `create_component`: `Create and store a custom component for the tenant: a native scene that arranges its declared images and videos as tiles in 3D space. Retur…`
- `create_project`: `Create a new project — the unit you compose and render into. compose / apply_composition / create_render / the preview family all require a…`
- `create_render`: `Queue an MP4 render of a project's composition. Returns { id (renderId), status, warnings? } — 'warnings[]' carries non-fatal advisories (o…`
- `create_upload`: `Ingest a LOCAL file — bytes you hold, when there is no public URL to hand import_media (prefer import_media whenever the bytes already sit…`
- `create_webhook`: `Register a webhook so long-running jobs notify you instead of blocking on wait_job — the right pattern for fan-out/async agents. Pass url +…`
- `delete_brief`: `Delete a brief. Compose jobs already run from it are unaffected (they snapshot).`
- `delete_composition`: `Delete a composition (and its version history) from a project. REFUSES the ACTIVE composition (409) — make another one active first, or del…`
- `delete_critic`: `Delete a registered critic by its criticId. It stops running in the Director gates and score_composition immediately.`
- `delete_media`: `Permanently delete a media item from your library (cleanup). Irreversible. Compositions referencing it will fail to render — only delete me…`
- `delete_project`: `Permanently delete a project you created (cleanup). Removes its composition and render history. Irreversible — only call on a project you o…`
- `delete_webhook`: `Delete a webhook subscription (stop receiving its deliveries). Irreversible — the signing secret is invalidated.`
- `derive_composition`: `Derive a reframed SIBLING composition for a different aspect ratio (the agent-native Auto-Reframe / Magic-Resize). Pass projectId + body {…`
- `describe_composition_ops`: `Discover the exact CompositionOp vocabulary accepted by apply_composition. Omit type for a compact list of operation names and descriptions…`
- `extract_brand_kit`: `Queue brand-token extraction from a website URL — ASYNC: returns a jobId immediately; then wait_job(kind="brand_kit_extract", id=jobId) for…`
- `finalize_upload`: `Finalize a direct upload once you have PUT the bytes to the uploadUrl from create_upload. Confirms the bytes landed and starts ingest: imag…`
- `generate_media`: `Generate one first-class Library media item from a prompt. Choose generator: text-to-video / text-to-image / image-to-video / text-to-music…`
- `get_account`: `ORIENT FIRST — show THIS key's account before you spend a metered call: the org it is bound to, the current plan, a per-feature entitlement…`
- `get_brief`: `Read a brief by id — the persisted intent plus its current quote (compose + estimated render).`
- `get_checkpoint`: `Read a checkpoint packet — the durable approval unit a held compose pauses at (wait_job reports awaiting_input with {checkpointId, stage, v…`
- `get_component_source`: `Read an exact component source as complete JSON. Supply sourceVersionId from the selected catalog card to read that immutable revision, ret…`
- `get_composition`: `READ BACK a composition as JSON — the edit itself: tracks, clips, card HTML, reframe segments, captions, markers, format. This is what crea…`
- `get_media_context`: `Fetch bounded authoring context for a media item: dimensions/thumbnail, compact face roster, transcript counts/sample, temporal grids, and…`
- `get_media_facts`: `Read prepared subject tracks and behind-subject mattes for one media item. For an exact readiness check, pass kind + startSec + endSec toge…`
- `get_profile`: `The org's legible taste in ONE read: brand kits, registered critics (the machine-checkable standard both the Director's gates and score_com…`
- `get_transcript`: `Read exact source-time transcript words in bounded utterance pages. Word start/end values are seconds from the source media start. Pass lim…`
- `get_usage`: `The A2 usage ledger: every metered billing event newest-first with attribution — featureId, amount, the project/job that produced it, and t…`
- `import_media`: `Import a media item into your library from a public URL — the agent-friendly ingest path (single call, no upload protocol). Pass url (https…`
- `import_resource`: `Import a stock candidate (candidateId from search_resources) into a project as an ORG-OWNED media item — provider/externalId/license proven…`
- `list_briefs`: `List briefs. DEFAULT shows human-authored briefs only; kind:"clip" shows the machine-minted clip briefs (suggest_briefs output), kind:"all"…`
- `list_catalog`: `Use projection:'component-library' for the unified source-free library page, returned as complete JSON with exact scoped definition/preset/…`
- `list_checkpoints`: `List checkpoint packets newest-first (filter with composeJobId for one run's v1→vN gate history, or projectId). The version stack with per-…`
- `list_compositions`: `List every composition (video) in a project, with its format and which one is active. Use a returned compositionId with create_render(compo…`
- `list_critics`: `List registered critics: criticId, label, tier (rules/rubric/evaluator), phase, floor, referenceMediaIds. Rubric text / rules / evaluator U…`
- `list_media`: `List the media in your CueFrame library. Filter a real library with kind (video/audio/image/gif/asset/source/stock), source (upload/generat…`
- `list_plans`: `List the plan catalog (tiers, intervals, product ids, prices) BEFORE a checkout, so create_checkout requests a real {plan, interval} instea…`
- `list_projects`: `List your projects — re-orient in an existing workspace instead of minting duplicates (steady-state entry, A9). Each row carries the id eve…`
- `list_render_fonts`: `The fonts the RENDERER can actually draw — read this BEFORE authoring type, not after a refusal. Per family: the exact family name authorin…`
- `new_composition`: `Create a NEW composition (a new video) inside a project — a project is a workspace that holds many videos. Returns { compositionId, format,…`
- `prepare_media`: `Prepare the perception artifact an authored edit needs BEFORE sighted review. Pass body.kind="subjectTrack" for face/active-speaker reframi…`
- `preview_card`: `Render ONE authored card on its own and SEE it, before placing it in a composition. Pass the same 'html' (+ optional 'tokens') you would pu…`
- `preview_clip`: `Render a scoped, cheap MOTION preview — ONLY body.fromSec→body.toSec of the composition (max 60s) at preview quality (capped resolution, li…`
- `preview_component`: `Queue a typed preview artifact for ONE org-installed component — ASYNC: returns a jobId immediately; then wait_job(kind="preview", id=jobId…`
- `preview_frame`: `Queue durable still-frame evidence for layout/copy judgment. Returns immediately with {jobId, kind:'preview_frame', status}; then call wait…`
- `register_critic`: `Register a custom eval into the compose critic panel — the critic contract is { rubric (or rules/evaluator), referenceMediaIds?, floor }. T…`
- `repin_component`: `Move clips that pin a retired TSX (version 3) component to its native (version 4) successor: the 'successorSourceVersionId' that get_compos…`
- `resolve_builtin_component`: `Resolve a selected builtin component-library card using its exact collection, id and revision. Returns the canonical pinned document and so…`
- `resume`: `Answer the checkpoint packet wait_job reported as awaiting_input (its {checkpointId} — read the packet FIRST with get_checkpoint and relay…`
- `retry_render`: `Re-render an existing render job's FROZEN composition snapshot — it inherits that job's exact composition/intent/priority and queues a fres…`
- `score_composition`: `Queue the durable server-side judge — it snapshots the exact authored target, samples eval beats, captures frames asynchronously, and grade…`
- and 12 more in [b25e350a1ddb55a63705.json](b25e350a1ddb55a63705.json)

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://api.cueframe.ai/v1/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
