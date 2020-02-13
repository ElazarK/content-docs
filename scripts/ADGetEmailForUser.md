`Deprecated`

Use Active Directory to retrieve the email address associated with the specified user. The user can be specified by "name", "email" or as an "Active Directory Distinguished Name" (DN).

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
| attributes | Include these AD attributes of the resulting objects in addition to the default ones. |

## Outputs
---
There are no outputs for this script.
