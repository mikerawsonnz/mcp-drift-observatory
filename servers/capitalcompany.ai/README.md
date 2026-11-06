# capitalcompany.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/capitalcompany.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://capitalcompany.ai/mcp` | 14 | [`19a51f4844d9`](62d6b0cca4647fe5fa82.json) | 2026-10-24 |

## Tools at `https://capitalcompany.ai/mcp`

- `capital_company_ask`: `Use this when the user asks about their own funds on Capital Company, or how Capital Company works. Answers a question about the user’s tea…`
- `capital_company_claim`: `For someone without a Capital Company account who said yes to a proposal: emails a sign-in link to the address they give. Opening the link…`
- `capital_company_confirm`: `Sends the user’s answer, confirm or decline, to a Confirmation from Capital Company. Confirming carries out what it describes; declining ca…`
- `capital_company_conversation`: `Reads the user’s current conversation with Capital Company, including the outcome of anything they confirmed and whether it is waiting on t…`
- `capital_company_create_commitment`: `Use this when the user wants to record that an investor committed to one of their funds. Starts recording the new commitment. Returns Capit…`
- `capital_company_create_fund`: `Use this when the user wants to set up an SPV or a fund — to pool investors’ money into one deal, such as buying a startup’s or a pre-IPO c…`
- `capital_company_edit_commitment`: `Use this when the user wants to change an investor’s existing commitment in one of their funds. Starts an edit to the fields they name. Ret…`
- `capital_company_invite_investors`: `Use this when the user wants to bring investors into one of their funds. Starts an invitation of investors to the fund by email address. Re…`
- `capital_company_reply`: `Sends the user’s answer to Capital Company’s last question, in their own words. Returns Capital Company’s next question, or a proposal for…`
- `capital_company_send_capital_calls`: `Use this when the user wants a fund’s investors to pay in money they committed. Starts capital call notices to the investors of a fund clas…`
- `capital_company_send_subscription_agreements`: `Use this when the user wants investors in one of their funds to sign their subscription agreements. Starts the signature requests. Returns…`
- `capital_company_show_confirmation`: `Shows a Confirmation from Capital Company on its card, where the user can confirm or decline it. Changes nothing.`
- `capital_company_update_fund`: `Use this when the user wants to change a setting on one of their funds. Starts a change to the settings they name. Returns Capital Company’…`
- `create_workspace`: `Use this when someone without a Capital Company account wants one for their firm. Opens a Capital Company workspace, an account and the fir…`

## Changes

- 2026-10-24: [description changed](../../deltas/2026-10-24/62d6b0cca4647fe5fa82.json): `9 field(s) changed`
- 2026-10-23: [annotation changed, description changed, field changed](../../deltas/2026-10-23/62d6b0cca4647fe5fa82.json): `7 field(s) changed; signals: length_more_than_doubled`
- 2026-10-22: [count changed, tool removed](../../deltas/2026-10-22/62d6b0cca4647fe5fa82.json): `3 tool(s) removed`
- 2026-10-20: [annotation changed, description changed](../../deltas/2026-10-20/62d6b0cca4647fe5fa82.json): `17 field(s) changed`
- 2026-10-18: [count changed, tool added](../../deltas/2026-10-18/62d6b0cca4647fe5fa82.json): `1 tool(s) added`
- 2026-10-16: [count changed, tool added](../../deltas/2026-10-16/62d6b0cca4647fe5fa82.json): `2 tool(s) added`

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://capitalcompany.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
