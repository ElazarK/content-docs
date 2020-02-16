`Deprecated`

Use Active Directory to check to see if the specified user is a member of the specified group. A simple yes or no answer will be returned. The user can be specified by name, email or as an Active Directory Distinguished Name (DN).

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | active directory, Condition |
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
| groupname | The name of the AD group to check. |
| nestedSearch | The value to enter (any amount) allow nested groups check as well. |

## Outputs
---
There are no outputs for this script.
