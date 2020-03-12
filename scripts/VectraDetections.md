---
id: vectra-detections
title: Vectra Detections (Deprecated)
---

`Deprecated`

Detects objects that contain all the information related to security events that are detected on the network. 

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
* vec-detections

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| fields | The filtered objects listed. |
| page | The page number. The possible values are, a positive integer, or last. |
| page_size | The page size. The possible values are, a positive integer, or all. |
| ordering | The orders records by last timestamp, threat score and certainty score. The default out sorts threat and certainty score in ascending order. Scores can be sorted in descending order by prepending the query with “minus” symbol. |
| min_id | The ID procided is less than or equal to ">=". |
| max_id | The ID provided is Greater than or equal to "<=". |
| state | The state to filter by. Can be, "active", "inactive", "ignored", or "ignored for all". |
| type_vname | The detection type to filter by (verbose name). |
| category | The detection category to filter by.  |
| src_ip | The source to filter by (IP address). |
| t_score | The threat score to filter by. |
| t_score_gte | The threat score >= the score provided to filter by.  |
| c_score | The certainty score to filter by.  |
| c_score_gte | The certainty score >= the score provided to filter by.  |
| last_timestamp | The last timestamp to filter by. |
| host_id | The ID of the host object a detection is attributed to filter by. |
| tags | The tag or a comma-separated list of tags to filter by. |
| destination | The destination in the detection detail set to filter by. |
| proto | The protocol in the detection detail set to filter by.  |
| dst_port | The destination port in the detection detail set to filter by. |
| inbound_ip | The `inbound_ip` in the relayed comm set to filter by.  |
| inbound_proto | The `inbound_proto` in the relayed comm set to filter by.  |
| inbound_port | The `inbound_port` in the relayed comm set to filter by.  |
| inbound_dns | The `inbound_dns` in the relayed comm set to filter by.  |
| outbound_ip | The `outbound_ip` in the relayed comm set to filter by. |
| outbound_proto | The `outbound_proto` in the relayed comm set to filter by.  |
| outbound_port | The `outbound_port` in the relayed comm set to filter by.  |
| outbound_dns | The `outbound_dns` in the `relayed_comm_set` to filter by.  |
| dns_ip | The `dns_ip` in the `dns_set` to filter by.  |
| dns_request | The `dns_request` in the `dns_set` to filter by.  |
| resp_code | The `resp_code` in the `dns_set` to filter by.  |
| resp | The `resp_in` the `dns_set` to filter by.  |

## Outputs
---
There are no outputs for this script.
