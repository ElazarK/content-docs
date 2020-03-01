---
id: ad-get-computer
title: AD Get Computer
---


`Deprecated` 

Use the `ad-get-computer` command in the Active Directory Query v2 instead.

Use Active Directory to retrieve detailed information about a computer account. The computer can be specified by "name", "email", or as an "Active Directory Distinguished Name" (DN).
If no filters are provided, the result will show all computers.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | active directory, enhancement, hostname |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* ad-search

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| dn | The Active Directory Distinguished Name for the desired computer. |
| name | Name of the desired computer |
| attributes | Include these AD attributes of the resulting objects in addition to the default ones. |
| customFieldType | Searches the computer by this custom field type. |
| customFieldData | Searches the computer by this custom field data (relevant only if the `customFieldType` is provided). |
| headers | The columns headers to show by order. |
| nestedSearch |  Enter "true" to allow nested groups to be searched as well. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Endpoint | The Active Directory endpoint. | Unknown |
| Endpoint.Type | The type of the endpoint entity. | Unknown |
| Endpoint.ID | The unique endpoint DN (Distinguished Name). | Unknown |
| Endpoint.Hostname | The endpoint hostname. | Unknown |
| Endpoint.Groups | The groups the endpoint is part of. | Unknown |
