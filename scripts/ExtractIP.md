---
id: extract-ip
title: Extract IP (Deprecated)
---

`Deprecated`

Deprecated - We recommend using `extractIndicators` command instead. 

Extracts IP addresses from the given text and places them both as output and in the context of a playbook.

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
| text | The text to extract the IP address from, and if the object will convert to JSON. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| IP.Address | The extracted IP addressess. | Unknown |
