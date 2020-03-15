---
id: cp-block-ip
title: CP Block IP (Deprecated)
---

`Deprecated`

Blocks one or more IP addresses using Checkpoint Firewall.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | checkpoint, firewall, response |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* checkpoint

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| ip | The one or more IP addresses to be blocked (comma-separated). |
| direction | Whether to block traffic "to" or "from" the IP addresses, or "both". The default is "both". |
| rulename | The base name for added rules inside checkpoint db. |
| ipname | The base name for added IP addresses/hosts inside checkpoint db. |

## Outputs
---
There are no outputs for this script.
