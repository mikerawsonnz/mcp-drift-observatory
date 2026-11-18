# www.aim-shield.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/www.aim-shield.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://www.aim-shield.ai/mcp` | 10 | [`1771e5a47b33`](89b62f82cc23b3feb966.json) | 2026-11-18 |

## Tools at `https://www.aim-shield.ai/mcp`

- `antes_de_actuar`: `Para agentes de IA que actúan en nombre de una persona. Antes de pagar, rellenar datos, iniciar sesión o descargar algo, pásanos el enlace…`
- `comprobar_cuenta_bancaria`: `Dice si un IBAN es válido, de qué país y banco es y, si das la cuenta de siempre, si el cambio es sospechoso. Úsalo antes de pagar a una cu…`
- `comprobar_mensaje`: `Dice si un mensaje (SMS, correo, WhatsApp), un enlace o un texto tiene señales de estafa, por qué y qué hacer. Pega el texto tal cual lo re…`
- `cortafuegos_de_ia`: `Para chatbots y agentes de una empresa. Con «entrada», pásanos lo que escribió una persona antes de dárselo a la IA: detecta intentos de sa…`
- `estado_de_mi_empresa`: `Con la clave del panel de empresa: la nota y las mejoras pendientes, el vigía del dominio, quién tiene acceso al panel y lo comprobado en T…`
- `foto_de_seguridad`: `La nota de 0 a 100 del correo, la web y el dominio de una empresa, mirando solo lo público, con las tres mejoras que más la protegen.`
- `preguntar_al_copiloto`: `Con la clave del panel de empresa: responde preguntas como «¿qué arreglo primero?», «¿cómo está el vigía?» o «¿quién tiene acceso?».`
- `registro_de_actividad`: `Con la clave del panel de empresa: lo último que se ha hecho en el panel (quién, qué y cuándo).`
- `repetir_foto_de_mi_empresa`: `Con la clave del panel de empresa: vuelve a mirar el dominio de la empresa y guarda la nota nueva en el panel (queda en el registro).`
- `revisar_servidor_mcp`: `Para quien va a conectar un servidor MCP a un agente. Pásanos la lista de herramientas del servidor (el JSON de «tools/list») y devuelve «p…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://www.aim-shield.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
