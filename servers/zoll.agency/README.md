# zoll.agency: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/zoll.agency.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://zoll.agency/mcp` | 8 | [`025349c7bd47`](4a6b54c7b92fc67af28d.json) | 2026-11-11 |

## Tools at `https://zoll.agency/mcp`

- `ausfuhranmeldung_noetig`: `Der Satz der Vorprüfung von zoll.agency für Bestimmungsland, Warenwert und Gewicht der ganzen Lieferung, nach der Grenze von 1.000 EUR und…`
- `einfuhr_weg_bestimmen`: `Der Einfuhr-Wegweiser von zoll.agency: Für eine Sendung aus einem Land außerhalb der EU, nach Empfänger (Firma oder privat), Versandweg (Po…`
- `incoterms_waehlen`: `Ordnet Antworten zu Transportweg, Fracht, Gefahrübergang, Versicherung, Einfuhrabgaben und Abladen einer Klausel der Incoterms® 2020 zu, mi…`
- `kumulierung_pruefen`: `Darf Vormaterial aus einem Partnerland der EU für den Ursprung der fertigen Ware zählen, wenn sie in ein bestimmtes Land verkauft wird? Nac…`
- `praeferenznachweis_bestimmen`: `Welcher Präferenznachweis gilt für die Ausfuhr aus der EU in ein Land (EUR.1, A.TR, Erklärung zum Ursprung auf der Rechnung, REX), mit Wert…`
- `ratgeber_suchen`: `Sucht in den Seiten von zoll.agency zu Einfuhr und Ausfuhr (Ratgeber, Themen, Werkzeuge, Leistungen) wie das Suchfeld der Seite und gibt hö…`
- `vorpruefung`: `Die Vorprüfung von zoll.agency mit den Angaben einer Handelsrechnung, die der Assistent aus der Rechnung übernimmt: Versender und Empfänger…`
- `warennummer_suchen`: `Sucht mit Wörtern oder einer Nummer (2 bis 11 Ziffern) in der Kombinierten Nomenklatur und zeigt höchstens 10 Codes mit dem amtlichen Wortl…`

## Changes

- 2026-11-11: [annotation changed, description changed, field changed](../../deltas/2026-11-11/4a6b54c7b92fc67af28d.json): `3 field(s) changed`
- 2026-11-10: [count changed, description changed, tool added, tool removed](../../deltas/2026-11-10/4a6b54c7b92fc67af28d.json): `2 tool(s) added; 1 tool(s) removed; 3 field(s) changed; signals: length_more_than_doubled`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://zoll.agency/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
