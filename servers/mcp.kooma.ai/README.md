# mcp.kooma.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/mcp.kooma.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://mcp.kooma.ai/mcp` | 4 | [`7d146ed07566`](f7a0977ce5f17ff1ff98.json) | 2026-08-26 |

## Tools at `https://mcp.kooma.ai/mcp`

- `kooma_list_voices`: `Liste les voix bambara disponibles pour la synthese vocale, avec leur identifiant, leur nom et leur genre. A appeler avant kooma_text_to_sp…`
- `kooma_text_to_speech`: `Transforme un texte en audio avec une voix bambara. Renvoie l'audio. Utiliser kooma_list_voices pour obtenir un identifiant de voix valide.`
- `kooma_transcribe_from_url`: `Transcrit en texte un fichier audio ou video accessible par une URL publique en HTTPS. La langue est detectee automatiquement. Le fichier e…`
- `kooma_translate`: `Traduit un texte entre le bambara et 13 autres langues. Les codes de langue combinent langue et ecriture : bam_Latn (bambara), fra_Latn (fr…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://mcp.kooma.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
