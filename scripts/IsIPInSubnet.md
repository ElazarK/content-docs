---
id: is-ip-in-subnet
title: Is IP In Subnet (Deprecated)
---

`Deprecated`

Returns 'yes' if the IP address is in subent. Otherwise it will return 'no'.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | Condition |
| Demisto Version | 0.0.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| ip | The IP address to check. |
| subnet | The IP address or subnet to check against. For example, "127.0.0.1 or 127.0.0.1/8". |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| True | If the IP address is in subnet. | Unknown |
| False | If the IP address is not in the subnet. | Unknown |
