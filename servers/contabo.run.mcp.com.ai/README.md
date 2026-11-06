# contabo.run.mcp.com.ai: declared MCP tools

Observed by the [MCP Drift Observatory](../../README.md). We record what this server **declared** (tool names, descriptions, schemas), byte-exactly, and when that changed. Declarations, not behaviour.

**Follow changes to this server:** [Atom feed](https://github.com/mikerawsonnz/mcp-drift-observatory/commits/main/servers/contabo.run.mcp.com.ai.atom): one entry each time its declared tools change, nothing otherwise.

| Endpoint | Tools | Hash | Declared since |
|---|---|---|---|
| `https://contabo.run.mcp.com.ai/mcp` | 124 | [`43115bc0bb33`](693771c9d5cb4dc2ca25.json) | 2026-08-20 |

## Tools at `https://contabo.run.mcp.com.ai/mcp`

- `CancelObjectStorage`: `Cancels the specified object storage at the next possible date - Cancels the specified object storage at the next possible date. Please be…`
- `assignInstancePrivateNetwork`: `Add instance to a Private Network - Add a specific instance to a Private Network`
- `assignIp`: `Assign a VIP to an VPS/VDS/Bare Metal - Assign a VIP to a VPS/VDS/Bare Metal using the machine id.`
- `bulkDeleteDnsZoneRecords`: `Bulk delete DNS zone records - Delete multiple zone records from a DNS Zone`
- `cancelDomain`: `Cancel a specific domain - Cancel a specific domain`
- `cancelInstance`: `Cancel specific instance by id - Your are free to cancel a previously created instance at any time.`
- `confirmDomainTransferOut`: `Confirm transfer out for a domain - Confirm transfer out for a domain`
- `createAssignment`: `Create a new assignment for the tag - Create a new tag assignment. This marks the specified resource with the specified tag for organizing…`
- `createCustomImage`: `Provide a custom image - In order to provide a custom image please specify an URL from where the image can be directly downloaded. A custom…`
- `createDnsZone`: `Create DNS zone - Creates a new DNS zone for a customer`
- `createDnsZoneRecord`: `Create DNS zone record - Create resource record in a zone`
- `createHandle`: `Create specific handle - Create specific handle`
- `createInstance`: `Create a new instance - Create a new instance for your account with the provided parameters. <table> <tr><th>ProductId</th><th>Product</th>…`
- `createObjectStorage`: `Create a new object storage - Create / purchase a new object storage in your account. Please note that you can only buy one object storage…`
- `createPrivateNetwork`: `Create a new Private Network - Create a new Private Network in your account.`
- `createPtrRecord`: `Create a new PTR Record using ip address - Create a new PTR Record using ip address. Only IPv6 can be created`
- `createRole`: `Create a new role - Create a new role. In order to get a list availbale api enpoints (apiName) and their actions please refer to the GET ap…`
- `createSecret`: `Create a new secret - Create a new secret in your account with attributes name, type and value. Attribute type can be password or ssh.`
- `createSnapshot`: `Create a new instance snapshot - Create a new snapshot for instance, with name and description attributes`
- `createTag`: `Create a new tag - Create a new tag in your account with attribute name and optional attribute color.`
- `createUser`: `Create a new user - Create a new user with required attributes name, email, enabled, totp (=Two-factor authentication 2FA), admin (=access…`
- `deleteAssignment`: `Delete existing tag assignment - Tag assignment will be removed from the specified resource. If this tag is being used for access restricti…`
- `deleteDnsZone`: `Delete a DNS zone. - Delete a DNS Zone using zone name.`
- `deleteDnsZoneRecord`: `Delete a DNS zone record - Delete a DNZ Zone's record`
- `deleteImage`: `Delete an uploaded custom image by its id - Your are free to delete a previously uploaded custom images at any time`
- `deletePrivateNetwork`: `Delete existing Private Network by id - Delete existing Virtual Private Cloud by id and automatically unassign all instances from it`
- `deletePtrRecord`: `Delete a PTR Record using ip address - Delete a PTR Record using ip address. Only IPv6 can be deleted`
- `deleteRole`: `Delete existing role by id - You can't delete a role if it is still assigned to a user. In such cases please remove the role from the users.`
- `deleteSecret`: `Delete existing secret by id - You can remove a specific secret from your account.`
- `deleteSnapshot`: `Delete existing snapshot by id - Delete existing instance snapshot by id`
- `deleteTag`: `Delete existing tag by id - Your tag can be deleted if it is not assigned to any resource on your account. Check tag assigments before dele…`
- `deleteUser`: `Delete existing user by id - By deleting a user he will not be able to access any endpoints or resources any longer. In order to temporaril…`
- `generateClientSecret`: `Generate new client secret - Generate and get new client secret.`
- `getAuthCode`: `Get auth code for a domain - Get auth code for a domain by id`
- `getObjectStorageCredentials`: `Get S3 compatible object storage credentials. - Get S3 compatible object storage credentials for accessing it via S3 compatible tools like…`
- `listDomains`: `List all domains - List and filter all your domains`
- `listHandles`: `List all handles - List and filter all your handles`
- `listObjectStorageCredentials`: `Get list of S3 compatible object storage credentials for user. - Get list of S3 compatible object storage credentials for accessing it via…`
- `orderDomain`: `Create or transfer a domain - Create or transfer a domain`
- `patchInstance`: `Update specific instance - Update specific instance by instanceId.`
- `patchPrivateNetwork`: `Update a Private Network by id - Update a Private Network by id in your account.`
- `regenerateObjectStorageCredentials`: `Regenerates secret key of specified user for the S3 compatible object storages. - Regenerates secret key of specified user for the a specif…`
- `reinstallInstance`: `Reinstall specific instance - You can reinstall a specific instance with a new image and optionally add ssh keys, a root password or cloud-…`
- `removeHandle`: `Remove specific handle - Remove specific handle`
- `rescue`: `Rescue a compute instance / resource identified by its id - You can reboot your instance in rescue mode to resolve system issues. Rescue sy…`
- `resendEmailVerification`: `Resend email verification - Resend email verification for a specific user`
- `resetPassword`: `Send reset password email - Send reset password email for a specific user`
- `resetPasswordAction`: `Reset password for a compute instance / resource referenced by an id - Reset password for a compute instance / resource referenced by an id…`
- `restart`: `Restart a compute instance / resource identified by its id. - To restart a compute instance that has been identified by its id, you should…`
- `retrieveApiPermissionsList`: `List of API permissions - List all available API permissions. This list serves as a reference for specifying roles. As endpoints differ in…`
- `retrieveAssignment`: `Get specific assignment for the tag - Get attributes for a specific tag assignment in your account. For this the resource type and resource…`
- `retrieveAssignmentList`: `List tag assignments - List and filter all existing assignments for a tag in your account`
- `retrieveAssignmentsAuditsList`: `List history about your assignments (audit) - List and filters the history about your assignments.`
- `retrieveCustomImagesStats`: `List statistics regarding the customer's custom images - List statistics regarding the customer's custom images such as the number of custo…`
- `retrieveDataCenterList`: `List data centers - List all data centers and their corresponding regions.`
- `retrieveDnsZone`: `Retrieve a DNS Zone by zone name - Get all attributes for a specific DNS Zone`
- `retrieveDnsZoneRecordsList`: `List a DNS Zone's records - Get all the records of a DNS Zone`
- `retrieveDnsZonesList`: `List DNS zones - Get a list of all zones`
- `retrieveDomain`: `List specific domain - List specific domain`
- `retrieveDomainsAuditsList`: `List history about your Domains (audit) - List and filters the history about your Domains.`
- and 64 more in [693771c9d5cb4dc2ca25.json](693771c9d5cb4dc2ca25.json)

## Changes

- None observed since we started watching.

## Check it from your agent

Free, no key, over MCP (`https://drift.getvda.ai/mcp`) or A2A (`https://drift.getvda.ai/a2a/`): call `drift_check` with

```json
{"action": "check", "url": "https://contabo.run.mcp.com.ai/mcp"}
```

It answers whether the declaration changed, when, and the Witness seal of our observation. Every crawl's changes across all servers: [the observatory's feed on the RSS-A board](https://hub.rssa.getvda.ai/network/@getvda-mcp-drift-observa-e131.atom?via=drift-page).

_Not affiliated with this server. Generated from the archive's own data._
