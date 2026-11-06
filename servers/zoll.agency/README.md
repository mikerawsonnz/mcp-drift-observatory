# zoll.agency: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/zoll.agency.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://zoll.agency/mcp` | 7 | [`5464b687cd35`](4a6b54c7b92fc67af28d.json) | 2026-10-25 |

## Tools at `https://zoll.agency/mcp`

- `ausfuhranmeldung_noetig`: `Der Satz der Vorprüfung von zoll.agency für Bestimmungsland, Warenwert und Gewicht der ganzen Lieferung, nach der Grenze von 1.000 EUR und…`
- `incoterms_waehlen`: `Ordnet Antworten zu Transportweg, Fracht, Gefahrübergang, Versicherung, Einfuhrabgaben und Abladen einer Klausel der Incoterms® 2020 zu, mi…`
- `kumulierung_pruefen`: `Darf Vormaterial aus einem Partnerland der EU für den Ursprung der fertigen Ware zählen, wenn sie in ein bestimmtes Land verkauft wird? Nac…`
- `leistungen_und_preise`: `Die Leistungen von zoll.agency mit einem Satz, dem Preis brutto und der Adresse der Seite, wie auf /leistungen.`
- `praeferenznachweis_bestimmen`: `Welcher Präferenznachweis gilt für die Ausfuhr aus der EU in ein Land (EUR.1, A.TR, Erklärung zum Ursprung auf der Rechnung, REX), mit Wert…`
- `ratgeber_suchen`: `Sucht in den Seiten von zoll.agency (Ratgeber, Themen, Werkzeuge, Leistungen) wie das Suchfeld der Seite und gibt höchstens 10 Treffer mit…`
- `warennummer_suchen`: `Sucht mit Wörtern oder einer Nummer (2 bis 11 Ziffern) in der Kombinierten Nomenklatur und zeigt höchstens 10 Codes mit dem amtlichen Wortl…`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://zoll.agency/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
