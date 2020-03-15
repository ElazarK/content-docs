---
id: data-hash-reputation-old
title: Data Hash Reputation Old (Deprecated)
---

`Deprecated`

Evaluates the reputation of a hash and returns a score between 0 and 3. Where 0 - unknown, 1 - known good, 2 - suspicious, 3 - known bad. If the indicator reputation was manually set, the manual value will be returned.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | reputation |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* file

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| input | Hash value to look up |
| forceCalc | The reputation to calculate, even if it is set to manual. Can be, "yes" or "no". |

## Outputs
---
There are no outputs for this script.
