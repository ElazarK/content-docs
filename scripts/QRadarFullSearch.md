---
id: qradar-full-search
title: QRadar Full Search (Deprecated)
---

`Deprecated`

Runs a QRadar query and returns its results to the War Room.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | QRadar |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* qradar-searches
* qradar-get-search-results
* qradar-get-search

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| query_expression | The query expressions in AQL. |
| fields | The fields to filter in. |
| timeout | The timeout in seconds. The default is 10 minutes. |
| interval | The interval to poll for results. The default is 10 seconds. |
| range | The number of results returned. |
| headers | The table headers. |

## Outputs
---
There are no outputs for this script.
