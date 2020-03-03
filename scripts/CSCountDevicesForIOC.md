---
id: cs-count-devices-for-ioc
title: CS Count Devices For IOC (Deprecated)
---

`Deprecated`

Lists the number devices that match each IOC in a query. This will be limited to SHA256, SHA1, MD5 hashes and domain types.

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
* cs-device-count-ioc

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| type | Selects one of the SHA256, SHA1, MD5, or domain. |
| value | The IOC to find. |

## Outputs
---
There are no outputs for this script.
