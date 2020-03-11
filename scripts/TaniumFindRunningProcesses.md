---
id: tanium-find-running-processes
title: Tanium Find Running Processes (Deprecated)
---

`Deprecated`

`TaniumAskQuestionComplex` is the same as the `AskQuestion` command with additional filtering prepared by the script (an XML subsection added to the request).

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | tanium |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* tn-result-info
* tn-result-data
* tn-add-question-complex

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| timeout | Forces Tanium to respond after a specified amount of time (in seconds) This will occur even if the data was not fully collected by Tanium. |
| processNamePrefix | The prefix of the process name to search for. |
| pollfreq | The poll  frequency (in seconds). |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Endpoint | The list of endpoints where the process was found. | Unknown |
