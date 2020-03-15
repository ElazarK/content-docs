---
id: elasticsearch
title: Elasticsearch (Deprecated)
---

`Deprecated`

Deprecated. Use the Elasticsearch v2 integration instead.

Runs a search query using Elasticsearch.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | Elasticsearch |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* search

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| explain | Computes a score explanation for a query and a specific document. The default is "false". |
| fields | The fields to fetch. Leave this empty to fetch the entire document. |
| index | The index name(s) to query (comma-separated). |
| query | The search query. |
| page | The page number to start search from. The default is 0. |
| size | The page size. Can be a number including and between 1 - 10000. The default is 100. |
| sort | The field to sort by. [:order], order = true for ascending. The default is "true". |

## Outputs
---
There are no outputs for this script.
