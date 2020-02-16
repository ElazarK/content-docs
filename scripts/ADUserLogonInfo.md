`Deprecated`

Use Active Directory to retrieve detailed information about a user account. The user can be specified by name, email or as an Active Directory Distinguished Name (DN).

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
| dn | The Active Directory Distinguished Name for the desired user. |
| name | The name of the desired user. |
| email | The email address of the desired user. |
| attributes | The AD attributes  to include of the resulting objects in addition to the default ones. |

## Outputs
---
There are no outputs for this script.
