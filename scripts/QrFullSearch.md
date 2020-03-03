---
id: qr-full-search 
title: Qr Full Search (Deprecated)
---

`Deprecated`

Performs a full search through the QRadar advance query languages.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | QRadar |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* QrGetSearchResults
* qr-searches
* qr-get-search

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| query_expression | The query expressions in AQL. |
| fields | The fields to filter in. |
| timeout | The timeout in seconds. The default is 10 minutes. |
| interval | The interval to poll for results. The default is 10 seconds. |
| range | The number of results to return. |

## Outputs
---
There are no outputs for this script.
