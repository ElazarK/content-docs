---
id: d2-drop
title: D2 Drop
---

Drops a file to a target system by providing its path on the server. In most cases use `CopyFileD2` instead.
This is a utility agent script to be used inside server scripts. See `CopyFileD2` for an example.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | agent, util |
| Demisto Version | 0.0.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| destpath | The full filesystem path and filename under which to save the file. |
| files | The source file name. |
| force | The overwrite file. |

## Outputs
---
There are no outputs for this script.
