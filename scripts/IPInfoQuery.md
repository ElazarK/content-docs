---
id: ip-info-query
title: IP Info Query (Deprecated)
---

`Deprecated`

Queries `ipinfo.io` regarding an IP address and returns a table. If a specific field is selected, only the value for that field as a string will be returned.
## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | ipinfo |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* ipinfo_field

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| field | Retrieves only a specific field. (Optional) |
| ip | The IP address to query. For example, "!ip 1.1.1.1". |

## Outputs
---
There are no outputs for this script.
