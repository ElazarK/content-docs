---
id: ad-get-user-groups
title: AD Get User Groups (Deprecated)
---

`Deprecated`

Retrieves the groups in which the specified user is a member. The user can be specified by "name", "email" or as an "Active Directory Distinguished Name" (DN).

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
| dn | The Active Directory Distinguished Name of the desired user. |
| name | The name of the desired user. |
| email | The email address of the desired user. |
| attributes | Include these AD attributes of the resulting objects in addition to the default ones. |
| nestedSearch | The value to enter to allow nested groups search as well. |

## Outputs
---
There are no outputs for this script.
