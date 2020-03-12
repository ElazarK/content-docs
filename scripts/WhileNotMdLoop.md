---
id: while-not-md-loop
title: While Not MD Loop (Deprecated)
---

`Deprecated`

Loop over until some condition is fulfilled `(Contents (MD) != value)`.
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
| cmdArguments | The comma-separated list of command/automation arguments and values to run. For example, "key=val,key=val,key=val". |
| value | The value that `keyToWatch` needs to be equal to. |
| maxIterations | The maximum number of iteration loops to preform. The default is 100. |
| sleepTime | The time to sleep/wait between iterations (in seconds). The default is 10. |

## Outputs
---
There are no outputs for this script.
