---
id: epo-update-endpoints
title: EPO Update Endpoints (Deprecated)
---

`Deprecated`

Triggers an ePO client task to update the AV signatures for specific endpoints.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | epo |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* epo-command

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| endpoints | The names of the endpoints to update. |
| eposerver | The ePO instance to use. |
| retryAttempts | The number of times the server will attempt to send the task to the client. The default is 1. |
| retryIntervalInSeconds | The retry interval (in seconds). The default is 30. |
| abortAfterMinutes | The maximum number of minutes before aborting all attempts. The default is 5. |
| stopAfterMinutes | The maximum duration (in minutes) the client task is allowed to run. The defaults is 20. |
| randomizationInterval | The duration (in minutes) over which to randomly spread the execution of the task. The defaults is 0 (which will execute on all clients immediately). |

## Outputs
---
There are no outputs for this script.
