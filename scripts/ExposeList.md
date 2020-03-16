---
id: expose-list
title: Expose List (Deprecated)
---

`Deprecated`

Retruns the Demisto list.

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
| listName | The list to expose to the context. |
| contextKey | The key to expose the list to. The default is `lists.listName`. |
| query | The optional Demisto query to apply on the list. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| lists | The containing object for the lists that will contain the list names. | Unknown |
