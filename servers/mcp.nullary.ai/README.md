# mcp.nullary.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.nullary.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.nullary.ai/mcp` | 35 | [`08f1e0e02b7e`](bd2a384be367f2e3da45.json) | 2026-08-20 |

## Tools at `https://mcp.nullary.ai/mcp`

- `get_compound`: `A compound (structure, name, max clinical phase) + its full negative profile across modalities/sources.`
- `get_coverage`: `Per-modality and per-source coverage stats (honest Phase-1 numbers).`
- `get_finding_provenance`: `Full provenance + detail for a single finding by id.`
- `get_model_card`: `Per-target Layer-1 model card: training counts and held-out scaffold-split metrics (ROC-AUC, PR-AUC, Brier, calibration). Accepts a gene sy…`
- `get_target_landscape`: `Target 'graveyard' / exhaustion index: how many distinct compounds/agents have been tried against a target and failed, broken down by modal…`
- `list_models`: `Summary of the Layer-1 inactivity-scoring model registry: how many per-target models, split by family, and median scaffold-split ROC-AUC.`
- `list_top_targets`: `Coverage browse: the most heavily-pursued ('graveyard') targets, ranked by recorded negative findings. Optional family filter (kinase, gpcr…`
- `search_adc_linker_failures`: `ADC failures attributed to linker chemistry.`
- `search_admet_failures`: `Small-molecule ADMET failures.`
- `search_admet_failures_all_modalities`: `ADMET failures across ALL modalities.`
- `search_ancestry_specific_failures`: `Ancestry-specific CRISPR failures.`
- `search_bispecific_format_failures`: `Bispecific format/engineering failures.`
- `search_developability_failures`: `Antibody developability failures.`
- `search_drug_drug_interaction_failures`: `Drug-drug interaction failures.`
- `search_failed_adcs`: `ADCs that failed at any stage.`
- `search_failed_bispecifics`: `Bispecifics that failed at any stage.`
- `search_failed_clinical_antibodies`: `Discontinued/terminated clinical antibodies.`
- `search_failed_essentiality_screens`: `Non-dependency / failed essentiality screens.`
- `search_failed_guides`: `Failed/ineffective CRISPR guides.`
- `search_failed_oligonucleotides`: `ASOs/siRNAs that failed engagement/developability.`
- `search_failed_peptide_therapeutics`: `Failed peptide therapeutics.`
- `search_failed_protacs`: `PROTACs that failed degradation/ternary/permeability.`
- `search_failed_replications`: `Findings that failed to replicate.`
- `search_failed_selectivity`: `Small molecules that failed selectivity.`
- `search_failed_vaccines`: `Failed/terminated vaccines (by pathogen/indication).`
- `search_inactive_compounds`: `Inactive small-molecule compound-target pairs.`
- `search_indication_history`: `ALL failed approaches for an indication across every modality.`
- `search_mechanism_failures`: `Approaches that failed for a mechanism (by target).`
- `search_oligo_delivery_failures`: `Oligonucleotide delivery failures.`
- `search_pathogen_history`: `Vaccine + antimicrobial + antibody failures for a pathogen.`
- `search_peptide_stability_issues`: `Peptide stability/half-life failures.`
- `search_protac_e3_issues`: `PROTAC E3-ligase recruitment / ternary failures.`
- `search_safety_failures`: `Clinical/preclinical safety failures across modalities.`
- `search_target_history`: `ALL failed approaches against a target across every modality.`
- `search_vaccine_immunogenicity_failures`: `Failed vaccine immunogen designs.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.nullary.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
