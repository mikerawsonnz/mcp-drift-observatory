# petstore.run.mcp.com.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/petstore.run.mcp.com.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://petstore.run.mcp.com.ai/mcp` | 19 | [`d7724949e275`](492ab3499c1360aa6d14.json) | 2026-08-20 |

## Tools at `https://petstore.run.mcp.com.ai/mcp`

- `addPet`: `Add a new pet to the store. - Add a new pet to the store.`
- `createUser`: `Create user. - This can only be done by the logged in user.`
- `createUsersWithListInput`: `Creates list of users with given input array. - Creates list of users with given input array.`
- `deleteOrder`: `Delete purchase order by identifier. - For valid response try integer IDs with value < 1000. Anything above 1000 or non-integers will gener…`
- `deletePet`: `Deletes a pet. - Delete a pet.`
- `deleteUser`: `Delete user resource. - This can only be done by the logged in user.`
- `findPetsByStatus`: `Finds Pets by status. - Multiple status values can be provided with comma separated strings.`
- `findPetsByTags`: `Finds Pets by tags. - Multiple tags can be provided with comma separated strings. Use tag1, tag2, tag3 for testing.`
- `getInventory`: `Returns pet inventories by status. - Returns a map of status codes to quantities.`
- `getOrderById`: `Find purchase order by ID. - For valid response try integer IDs with value <= 5 or > 10. Other values will generate exceptions.`
- `getPetById`: `Find pet by ID. - Returns a single pet.`
- `getUserByName`: `Get user by user name. - Get user detail based on username.`
- `loginUser`: `Logs user into the system. - Log into the system.`
- `logoutUser`: `Logs out current logged in user session. - Log user out of the system.`
- `placeOrder`: `Place an order for a pet. - Place a new order in the store.`
- `updatePet`: `Update an existing pet. - Update an existing pet by Id.`
- `updatePetWithForm`: `Updates a pet in the store with form data. - Updates a pet resource based on the form data.`
- `updateUser`: `Update user resource. - This can only be done by the logged in user.`
- `uploadFile`: `Uploads an image. - Upload image of the pet.`

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://petstore.run.mcp.com.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
