Use this script to connect to a Checkpoint firewall appliance using SSH and retrieve status for backup tasks. The user account being that accesses the device must be set to use the SSH shell and not the built in Checkpoint CLI. Consult the Checkpoint documentation for instructions on how to do this.
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
| devices | The list of devices to backup (comma separated). |
| waittimeout | The wait time in seconds. If not provided, it will not wait. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| CheckpointBackup.DeviceName | The name of backed-up device. | Unknown |
| CheckpointBackup.System | The backed up system. | Unknown |
| CheckpointBackup.Status | The status of the backup process. | Unknown |
| CheckpointBackup.Path | The path of the backup file. | Unknown |
