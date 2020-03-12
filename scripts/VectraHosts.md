---
id: vectra-hosts
title: Vectra Hosts (Deprecated)
---

`Deprecated`

Includes host information data that correlates to the host data to the detected security events.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | Vectra |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* vec-hosts

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| fields | Filters the objects listed. |
| page | The page number. Possible values are, a positive integer, or last. |
| page_size | The page size. Possible values are, a positive integer, or all. |
| ordering | Orders the records by last timestamp, threat score and certainty score. The default out sorts threat and certainty score in ascending order. The scores can sorted in descending order by prepending the query with the “minus” symbol. |
| name | The name to filter by. |
| state | The state to filter by. Can be, "active", "inactive", "suspended", "ignored", or "ignored4all". |
| last_source | The "last_source" to filter by (IP address). |
| t_score | The threat score to filter by.  |
| t_score_gte | The threat score >= the score provided to filter by. |
| c_score | The certainty score to filter by. |
| c_score | The current certainty score integer correlated to the host |
| c_score_gte | The certainty score >= the score provided to filter by. |
| last_detection_timestamp | The `last_detection_timestamp` to filter by.  |
| tags | The tag or a comma-separated list of tags to filter by. This will return hosts that contain any of the tags specified. For example, "tags=baz | tags=foo,bar". |
| key_assest | The key asset to filter by. Can be, "True" or "False". |
| mac_address | The mac address to filter by.  |

## Outputs
---
There are no outputs for this script.
