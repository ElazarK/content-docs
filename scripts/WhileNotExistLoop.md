---
id: while-not-exist-loop
title: While Not Exist Loop (Deprecated)
---

`Deprecated`

Loops until th `${keyToWatch}` field is in the context.

Make sure the timeout of the script is also sufficient for the loop.

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
| cmdToRun | The command or automation script to execute each, while the loop iterates. |
| cmdArguments | The comma-separated list of command/automation arguments and values to run. For example, "key=val,key=val,key=val". |
| keyToWatch | The key to watch. If it is equal to value argument `(${key}==value)` then it will exit the loop. Otherwise it will continue to next loop iteration. This will run the command again. |
| maxIterations | The maximum number of iteration loops to preform. The default is 100. |
| sleepTime | The time to sleep/wait between iterations (in seconds). The default is 10. |

## Outputs
---
There are no outputs for this script.

---
