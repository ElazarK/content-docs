---
id: ad-get-group-users
title: AD Get Group Users (Deprecated)
---

`Deprecated`

Retrieves the list of users who are members of the specified group. Group must be given by its AD Distinguished Name. The `attributes` argument receives a comma-separated list of additional attributes you wish to be displayed in the results.

Example usage: `!ADGetGroupUsers groupdn="CN=Domain Admins,CN=Users,DC=demisto,DC=com" attributes=badPwdCount,memberOf`

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

## Outputs
---
There are no outputs for this script.  
