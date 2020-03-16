---
id: extract-url
title: Extract URL (Deprecated)
---

`Deprecated`

Deprecated - We recommend using `extractIndicators` command instead. 

Extracts URLs from the given text and places them both as output and in the context of a playbook. If given an object, it will convert it to JSON.

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
| text | The text to extract URLs from, and if the object will convert to JSON. |
| urlRegex | The regex used to recognize URLs. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| URL.Data | The extracted URLs. | Unknown |
