---
id: nessus-get-report
title: Nessus Get Report (Deprecated)
---

`Deprecated`

Gets a report for a scan. This will trigger an export in the requested file format, and will then wait 5 minutes for it to complete (or the timeout given as an argument), and downloads the report.

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
* scan-export
* scan-report-download
* scan-export-status

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| scanId | The scan ID. Use the command `list-scans` to get possible scan ID's. |
| historyId | The `history_id` of the historical data that should be returned. |
| format | The scanned report file format. Can be, "nessus", "csv", "html", "db" or "pdf". The default is "nessus". |
| password | The password used to encrypt the database exports. This is required when exporting as a DB. |
| chapters | The chapters to include in the export. This expects a semi-colon delimited string comprised of a combination of the following options: "vuln_hosts_summary", "vuln_by_host", "compliance_exec", "remediations", "vuln_by_plugin", and "compliance". |
| timeout | The amount of time (in seconds) to wait for the result before giving up. The default is 5 minutes. |

## Outputs
---
There are no outputs for this script.
