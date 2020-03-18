---
id: nessus-create-scan
title: Nessus Create Scan (Deprecated)
---

`Deprecated`

Creates a new scan.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | nessus |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* scan-create

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| editor | The UUID for the template editor to use. |
| name | The name of the scan. |
| description | The description of the scan |
| policyId | The unique ID of the policy to use (number). |
| folderId | The unique ID of the destination folder for the scan (number). |
| scannerId | The unique ID of the scanner to use (number). |
| schedule | The schedule for the scan is enabled, i set to true. Can be, "true" or "false". |
| launch | Whether to launch the scan. For example, "ON_DEMAND", "DAILY", "WEEKLY", "MONTHLY", or "YEARLY". |
| startTime | The starting time and date for the scan. For example, "YYYYMMDDTHHMMSS". |
| rules | The semi-colon delimited string comprised of three values. The frequency, "FREQ=ONCE", "DAILY", "WEEKLY", "MONTHLY" or "YEARLY". The interval "INTERVAL=1", "2", "3" ..."x". The days of the week "BYDAY=SU", "MO", "TU", "WE", "TH", "FR" or "SA". To create a scan that runs every three weeks on Monday Wednesday and Friday the string would be 'FREQ=WEEKLY;INTERVAL=3;BYDAY=MO,WE,FR'. |
| timeZone | The timezone for the scan schedule. |
| targets | The list of targets to scan. Can be "single host" or "comma-separated targets". |
| emails | The comma separated list of accounts who will recieve the email summary report. |
| acls | The array containing permissions to apply to the scan. |
| fileTargets | The name of a file containing the list of targets to scan. |

## Outputs
---
There are no outputs for this script.
