---
id: cs-hunt-by-ioc
title: CS Hunt By IOC (Deprecated)
---

`Deprecated`

Lists devices that match a specific IOC. This means an IOC ran on them. This is limited to SHA256, SHA1, MD5 hashes, and domain types.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | crowdstrike |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* cs-device-ran-on

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| type | Selects one of the following SHA256, SHA1, MD5 hashes, or domain. |
| value | The IOC to find. |

## Outputs
---
There are no outputs for this script.
