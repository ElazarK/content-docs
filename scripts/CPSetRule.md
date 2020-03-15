---
id: cp-set-rule
title: CP Set Rule (Deprecated)
---

`Deprecated`

Sets attributes of an access rule object configured in Checkpoint firewall.
## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | checkpoint |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* checkpoint

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| uid | The UID of the rule. |
| name | The name of the rule. |
| layer | The layer of the rule. For example, "Network". |
| enabled | Wether to enable the rule, "true" to enable it, "false to disable it. |

## Outputs
---
There are no outputs for this script.
