---
id: extract-email
title: Extract Email (Deprecated)
---

`Deprecated`

Deprecated - We recommend using `extractIndicators` command instead. 

Extracts emails from the given text and places them both as output and in the context of a playbook. If given an object, it will convert it to JSON.

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
| text | The text to extract the emails from, and if the object will convert to JSON. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Account.Email.Address | The extracted emails. | Unknown |
