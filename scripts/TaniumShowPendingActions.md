---
id: tanium-show-pending-actions
title: Tanium Show Pending Actions (Deprecated)
---

`Deprecated`

Sends a request for a formatted result of a saved question. To receive the most up to date data, run the same command twice. See [here](https://kb.tanium.com/SOAP) for more information.

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

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| fulljson | Whether to return full json for each task instead of a table summary. True will make this occur. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Tanium.Action.Name | The name of the Action. | Unknown |
| Tanium.Action.State | The state of the Action. | Unknown |
| Tanium.Action.Comment | The Tanium comment. | Unknown |
| Tanium.Action.PackageName | The Tanium package name. | Unknown |
| Tanium.Action.PackageID | The Tanium package ID. | Unknown |
| Tanium.Action.AvailableTime | The Tanium available time. | Unknown |
