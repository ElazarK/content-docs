---
id: get-duplicates-ml
title: Get Duplicates Ml (Deprecated)
---

`Deprecated`

Finds duplicate incidents candidates.

Uses machine learning techniques with pre-defined data. This can also use data from the local environment. This script takes into consideration different features such as, "labels comparison", "email labels" (relevant for phishing), "incident time difference", and "shared indicators", which can be customized by the arguments.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | dedup, incidents, ml, duplicate |
| Demisto Version | 3.5.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| maxNumberOfIncidents | The maximum number of incidents to fetch from the database, to consider for machine-learning calculation. |
| timeFrameDays | The candidates to check for duplication in this time frame. Time frame is in number of days from after a specified time. |
| ignoreClosedIncidents | The closed incidents to ignore as potential candidates. |
| threshold | The threshold to consider as duplication of an incident. Must be a number between "0" and "1". |
| compareIndicators | The indicators to consider for duplicate calculation. Can be, "Email", "IP", "Domain", "File SHA256", "File MD5", or "URL". (CSV) |
| compareEmailLabels | The email labels to consider for duplicate calculation. Can be, "Email/headers/From", "Email/headers/Subject", "Email/text", "Email/html", or "Email/attachments". (CSV). If the labels are different from the default, specify the labels as follows, `LABEL_NAME:YOUR_LABEL_NAME`. For example, "email/from:email_sender". |
| compareOtherLabels | Whether to take into account all labels keys. |
| compareIncidentTimeDiff | Whether to take into account the incident time differences. |
| UseLocalEnvDuplicatesInLastDays | THe duplicate incident examples to consider from the local environment within the last "X" days. The default is "0", which means do not use. |
| ipComparisonSubnetMask | The equity to consider of the IP address base on this subnet mask. A valid value is a number between "0" and "32". THe default is "32", which means an exact match of the IP addresses. |
| maxCandidates | The maximum number of candidates in the output, in the incidents candidate list. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| duplicateCandidate | The duplicate candidate. | unknown |
| foundDuplicates | Whether any duplicates were found. | Unknown |
| duplicateCandidateList | The duplicate incident candidates list. | Unknown |
