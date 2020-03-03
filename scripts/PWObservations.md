---
id: pw-observations
title: PW Observations (Deprecated)
---

`Deprecated`

Queries for ProtectWise observations. Supports a comma-separated list of sensor IDs. This will query each sensor with the given parameters.

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
* observation-search

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| start | The timestamp of the start time of the event. The format can be, "1401451200000", or "ISO 8601" format (YYYY-MM-DDTHH:MM:S). For example, "2015-03-25T12:00:00". |
| end | The timestamp of the end of the event. Example: The format can be, "1401451200000", or "ISO 8601" format (YYYY-MM-DDTHH:MM:S). For example, "2015-03-25T12:00:00". |
| sensorId | The sensor ID or a comma-separated list of sensor IDs. |
| hasKillChain | Searches for observations in every kill chain stage. Can be, "true", or "false". |
| killChainStage | Filter by killchain stage. Can be, "Methodology", "Recon", "Delivery", "Exploit", "Beacon", "CnC", "Fortification", or "Data_Theft". |
| minLimit | The minimum results per page. |
| maxLimit | The maximum results per page. |
| type | Filters by the observation type. Can be, "ids", "http", "iprep", "urlrep", "protocol", or "file".  |
| ip | Filters observations by IP address in the `src`/`dst` fields. |
| threatLevel | Filters by Low, Medium, or High threats. Can be, "NONE", "LOW", "MEDIUM", or "HIGH". |
| threatCategory | Filter by threat category. Can be, "ExploitsAndAttacks", "DenialOfService", "Malware", "Scanning", "Botnets", "Phishing", "Suspicious", "MaliciousHost", "APT", "Misc", or "Unknown". |
| signatureId | Filters by threat signature. This finds observations of the same type of threat. For example, "69020504". |
| expandDetails | Includes observation records. Can be, "true" or "false". |
| reverseOrder | Returns results sorted by descending timestamp. The default is "true". |
| nextPage | The identifier that fetches the next page in the result set. |

## Outputs
---
There are no outputs for this script.
