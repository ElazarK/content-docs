---
id: design-best-practices
title: Integration Design Best Practices  (Deprecated)
---

`Deprecated`

Deprecated. Use the Elasticsearch v2 integration instead.

Runs an Elasticsearch query and displays the results in a table.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
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
| query | The ElasticSearch query to execute. |
| index | The index to check (supports wildcards). The Default is "*". |
| fields | The fields that should be included. Leave blank if you want all fields. |

## Outputs
---
There are no outputs for this script.
