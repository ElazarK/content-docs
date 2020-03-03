---
id: cs-indicators
title: CS Indicators (Deprecated)
---

`Deprecated`

Queries CrowdStrike indicators based on given parameters.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | server, threat-intel, crowdstrike |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* cs-indicators

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| parameter | The parameter to search by. Can be, indicator, type, report, actor, malicious_confidence, published_date, last_updated, malware_family, kill_chain, labels, DomainType, EmailAddressType, IntelNews, IPAddressType, Malware, Status, Target, ThreatType, Vulnerability. |
| filter | The was to filter. Can be, match, equal, gt(e), or lt(e). |
| value | The value for the given parameter. |
| sort | Sorts by a field. Should be "field_name.order" where order is either ascending or descending. Fields can be, indicator, type, report, actor, malicious_confidence, published_date, or last_updated. |
| page | The page to retrieve. (1 based) |
| pageSize | The size of the page to retrieve. |

## Outputs
---
There are no outputs for this script.
