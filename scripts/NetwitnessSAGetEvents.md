---
id: netwitness-sa-get-events
title: Netwitness SA Get Events
---

Returns all the RSA NetWitness SA events in the defined time range.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | RSA NetWitness Security Analytics |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* nw-get-events

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| timeRangeType | The filter of time range in which the events occured. |
| deviceId | The ID of the device where the events are stored or occurred. Run the command `nw-get-components` to get a list of available devices/components. (number) |
| collectionName | (optional) |
| predicateIds | (optional) |
| startDate | If timeRangeType defined as CUSTOM, set this argument. (optional datetime) |
| endDate | If timeRangeType defined as CUSTOM, set this argument. (optional datetime) |
| lastCollectionTime | The last collection time. (optional datetime) |
| mid1 | mID1 |
| mid2 | mID2 |
| investigationToken | The investigation ID token. (optional guid) |
| page | The page number. The default is set to 1. (optional number) |
| start | The starting index of event in page. The default is set to 0. (optional number) |
| limit | The limit on the number of events per page. The default is set to 25. (optional number) |

## Outputs
---
There are no outputs for this script.
