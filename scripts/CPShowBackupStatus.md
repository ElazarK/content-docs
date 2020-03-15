---
id: cp-show-backup-status
title: CP Show Backup Status (Deprecated)
---

`Deprecated`

Connects to a checkpoint firewall appliance using SSH and retrieve status for backup tasks. The user account being used to access the device must be set to use the SSH shell and not the built in Checkpoint CLI. 

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | checkpoint |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* ssh

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| devices | The list of devices to backup (commma-separated). |
| waittimeout | The wait time before timing out. (in seconds) If not provided, it does not wait. |

## Outputs
---
There are no outputs for this script.
