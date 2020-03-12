---
id: while-loop
title: While Loop (Deprecated)
---

`Deprecated`

Loops over until some condition is fulfilled `(${keyToWatch} == value)`.
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
| cmdToRun | The command or automation script to execute while the loop iterates. |
| cmdArguments | THe comma-separated list of command/automation arguments and values to run. For example, "key=val,key=val,key=val". |
| keyToWatch | The key to watch. If it is equal to the value argument `(${key}==value)` then it will exit the while loop. Otherwise  it will continue to the next loop iteration. This will run the command again. |
| value | The value that `keyToWatch` needs to be equal to. |
| maxIterations | The maximum numbers of iteration loop to preform. The default is 100. |
| sleepTime | The time to sleep/wait between iterations (in seconds). The default is 10. |

## Outputs
---
There are no outputs for this script.
