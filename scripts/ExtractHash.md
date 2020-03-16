---
id: extract-hash
title: Extract Hash (Deprecated)
---

`Deprecated`

Deprecated - We recommend using `extractIndicators` command instead. 

Extracts MD5, SHA1, SHA256 hashes from the given text and places them both as output and in the context of a playbook.

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
| text | The text to extract the hashes from, and if the object will convert to JSON. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| File.MD5 | The extracted MD5 hash of the file.| Unknown |
| File.SHA1 | The extracted SHA1 hash of teh file. | Unknown |
| File.SHA256 | The extracted SHA256 hash of the file. | Unknown |
