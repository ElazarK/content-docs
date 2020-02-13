`Deprecated`

Use Active Directory to retrieve the list of users or computers that are members of the specified group. Group must be given by its AD Distinguished Name. The `attributes` argument receives a comma-separated list of additional attributes you wish to be displayed in the results.

Example usage: `!ADGetGroupMembers memberType=user groupdn="CN=Administrators,CN=Builtin,DC=acme,DC=int" attributes=name,email`

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | active directory |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* ad-search

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| groupdn | The Active Directory Distinguished Name for the desired group. |
| attributes | Include these AD attributes of the resulting objects in addition to the default ones. |
| memberType | The member types to query.  |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Endpoint | The Active Directory endpoint. | Unknown |
| Endpoint.Type | The type of the endpoint entity. | Unknown |
| Endpoint.ID | The unique endpoint DN (Distinguished Name). | Unknown |
| Endpoint.Hostname | The endpoint hostname. | Unknown |
| Endpoint.Groups | The groups that the endpoint is part of. | Unknown |
| Account | The Active Directory account. | Unknown |
| Account.Type | The type of the account entity. | Unknown |
| Account.ID | The unique Account DN (Distinguished Name) | Unknown |
| Account.Username | The account username. | Unknown |
| Account.Email | The email address associated with the account. | Unknown |
| Account.Groups | The groups the account is part of. | Unknown |
| Account.DisplayName | The account display name. | Unknown |
