---
id: virustotal-is-malicious
title: Virustotal Is Malicious (Deprecated)
---

`Deprecated`

Queries Virustotal with a file hash.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | virustotal |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* file

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| hash | Checks only the files whose names are in the list, if provided. The names should be comma-separated. |
| threshold | Uses the default from Common/CommonUser thresholds, if not set. [vtPositives] |
| retries | The maximum amount of times to retry if it hits the rate limitation on the Virustotal key. It will retry every 1 min.|

## Outputs
---
There are no outputs for this script.
