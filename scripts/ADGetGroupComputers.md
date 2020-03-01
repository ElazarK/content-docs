---
id: ad-get-group-computers
title: AD Get Group Computers (Deprecated)
---

`Deprecated`

Use Active Directory to retrieve the list of computers that are members of the specified group. Group must be given by its AD Distinguished Name. The `attributes` argument receives a comma-separated list of additional attributes you wish to be displayed in the results.
Example usage: `!ADGetGroupComputers groupdn="CN=ImportantComputers,DC=demisto,DC=com" attributes=operatingsystem` 

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
| attributes | Include these AD attributes of the resulting objects in addition to the default ones |

## Outputs
---
There are no outputs for this script. 
