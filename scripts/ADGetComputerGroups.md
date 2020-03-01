---
id: ad-get-computer-groups
title: AD Get Computer Groups (Deprecated)
---

`Deprecated`

Use Active Directory to retrieve the groups in which the specified computer is a member. The member computer can be specified by name or by DN.

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
| dn | The Active Directory Distinguished Name for the desired computer. |
| name | The name of the desired computer. |
| attributes | Include these AD attributes of the resulting objects in addition to the default ones. |

## Outputs
---
There are no outputs for this script.
