`Deprecated`

Run Active Directory queries.

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
| filter |  (mandatory) Query the AD in AD syntax. For example, `(&(objectCategory=person)(objectClass=user)(!(cn=andy))` will find all user objects except andy. |
| baseDn | Root |
| attributes | The fields to specify that will be returned (comma separated). |
| sizeLimit | The maximum number of returned records. |
| timeLimit | The maximum time of query response (in seconds). |

## Outputs
---
There are no outputs for this script.
