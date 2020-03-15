---
id: cp-create-backup
title: CP Create Backup (Deprecated)
---

`Deprecated`

Connects to a Checkpoint firewall appliance using SSH and triggers a task to create a configuration backup of the device. The user account being used to access the device, must be set to use the SSH shell and not the built in Checkpoint CLI. 

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
| devices | The list of RemoteAccess instances of the checkpoint firewall appliances to back up. |

## Outputs
---
There are no outputs for this script.
