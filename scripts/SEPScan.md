---
id: sep-scan
title: SEP Scan (Deprecated)
---

`Deprecated`

This automation is deprecated, please use `sep-scan-endpoint` command in 'Symantec Endpoint Protection V2' integration.

Scans an IP address/hostname with Symantec Endpoint Protection. 

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | sep, symantec |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* sep-command-status

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| scanType | The type of scan. |
| ip | The IP address of the endpoint. |
| hostname | The hostname of the endpoint. |
| timeout | The timeout of the command. |
| interval | The polling interval of the command. |

## Outputs
---
There are no outputs for this script.
