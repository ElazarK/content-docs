---
id: locate-attachment
title: Locate Attachment (Deprecated)
---

`Deprecated`

Identifies whether the incident includes an attached file. The optional `typefilter` argument can be used to only match if the file type includes that string. This is the same for filename. The file type is according to the linux `file` command (filemagic format identification).

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | email, Condition |
| Demisto Version | 0.0.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| typefilter | The substring of the filetype to match. (Optional) |
| namefilter | The Substring of the file name to match. (Optional) |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| True | The incident has an attached file. | Unknown |
| False | The incident does not contain an attached file. | Unknown |
