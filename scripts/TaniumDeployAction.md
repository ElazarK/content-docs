---
id: tanium-deploy-action
title: Tanium Deploy Action (Deprecated)
---

`Deprecated`

Executes an action, optionally with parameters, and filterin, based on an existing package. Click [here](https://kb.tanium.com/SOAP) for more information.

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
* tn-deploy-package

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| packageName | Specifies the package name. For example, "!TaniumDeployAction packageName="Clean Stale Tanium Client Data"". |
| packageID | The package ID  that will be used instead of its name. |
| parameters | The parameters that wil be used with the package. Click [here](https://kb.tanium.com/SOAP) for more details. |
| comment | The comment to be added to the action history in the Tanium server. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Tanium.Action.ID | The ID of the action. | Unknown |
| Tanium.Action.Command | The command of the action. | Unknown |
| Tanium.Action.State | The state of the action. | Unknown |
| Tanium.Action.Comment | The Tanium comment. | Unknown |
| Tanium.Action.PackageName | The Tanium package name. | Unknown |
