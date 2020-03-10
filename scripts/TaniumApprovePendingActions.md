---
id: tanium-approve-pending-actions
title: Tanium Approve Pending Actions (Deprecated)
---

`Deprecated`

Approves all pending actions using the specified package names.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | tanium |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* tn-get-object
* tn-add-object

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| approvedpackages | The names of packages to approve. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Tanium.Action.Approve.Name | The action name. | Unknown |
| Tanium.Action.State | The action state. | Unknown |
| Tanium.Action.Comment | The tanium comment. | Unknown |
| Tanium.Action.PackageName | The tanium package name. | Unknown |
| Tanium.Action.PackageID | The tanium package ID. | Unknown |
