---
id: is-context-set
title: Is Context Set (Deprecated)
---

`Deprecated`

Checks if a context key is set. This can also optionally provide a value argument to compare against context data for this key.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | server, Utility, Condition |
| Demisto Version | 0.0.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| key | The key to check to see if it exists. |
| value | The optional value to compare to the context. If it is not provided it will check only the existence. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| True | If the given value exists in context. | Unknown |
| False | If the given value does not exist in context. | Unknown |
