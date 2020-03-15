---
id: design-best-practices
title: Integration Design Best Practices  (Deprecated)
---

`Deprecated`

Checks whether the given item is included in the whitelist.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | whitelist |
| Demisto Version | 0.0.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| item | The item to check. |
| whitelistname | The name of whitelist to check. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| WhitelistCheck | Returns a dictionary of indicators mapped to "True" if found in the whitelist, or "False" otherwise. | Unknown |
