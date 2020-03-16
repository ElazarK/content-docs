---
id: expose-users
title: Expose Users (Deprecated)
---

`Deprecated` 

Returns Demisto users.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | Utility |
| Demisto Version | 0.0.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| roles | The optional list of roles we want to get of users. Can be, "arrays" or "comma-separated" lists. |

## Outputs 
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| DemistoUsers.username | The username of the user. | Unknown |
| DemistoUsers.email | The email of the user. | Unknown |
| DemistoUsers.phone | The phone of the user. | Unknown |
| DemistoUsers.name | The name of the user. | Unknown |
| DemistoUsers.roles | The roles for the user. | Unknown |
