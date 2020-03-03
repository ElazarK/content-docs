---
id: pw-events
title: PW Events (Deprecated)
---

`Deprecated`

Retrieves events from ProtectWise. If the query does not include a time range, the default will be set to the last 24 hrs.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | protectwise |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* search

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| start | The timestamp of the start time of the event. The format can be, "1401451200000", or "ISO 8601 format" (YYYY-MM-DDTHH:MM:S), for example, "2015-03-25T12:00:00". |
| end | The timestamp of the end of the event. Example: The format can be, "1401451500000", or "ISO 8601 format" (YYYY-MM-DDTHH:MM:S) for example, "2015-03-25T12:00:00". |
| minLimit | The minimum amount of results per page to return. |
| maxLimit | The maximum amount of results per page to return.|
| ip | Filters by events that are affected by a specific IP address. |
| eventType | Filters by one or more event types. Can be, "MaliciousFlow", "KillChainEscalation", or "MaliciousConversation". |
| expandDetails | Whether to include observation records. Can be "true" or "false". |
| killChainStage | Filters by killchain stage. (Methodology Recon Delivery Exploit Beacon CnC Fortification Data_Theft) |
| nextPage | Fetches the next page in the result set. |
| observationStage | Filters by "Realtime" or "Retrospective". |
| reverseOrder | Returns results sorted by a descending timestamp. The default is "true". |
| threatCategory | Filters by threat category. Can be, "ExploitsAndAttacks", "DenialOfService", "Malware", "Scanning", "Botnets", "Phishing", "Suspicious", "MaliciousHost", "APT", "Misc", or "Unknown". |
| threatLevel | Filters by Low, Medium, or High threats. Can be, "NONE", "LOW", "MEDIUM"|, or "HIGH". |

## Outputs
---
There are no outputs for this script.
