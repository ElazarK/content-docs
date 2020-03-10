---
id: tanium-ask-question
title: Tanium Ask Question (Deprecated)
---

`Deprecated`

Sends a request for a formatted result of a saved question. To receive the most up to date data, run the same command twice. Click (here)[https://kb.tanium.com/SOAP] for more information.

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

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| name | Retrieves the question by its name. For example "!TaniumAskQuestion name="Running Services"". |
| id | Retrieves the question by its ID.  To view the ID in the Tanium console go to: **Authoring -> Saved Questions tab**. This will show you a list of saved questions. Click the **Edit** button on a saved question and the ID will appear in the lower left corner. |
| timeout | Forces Tanium to respond after a given amount of time (in seconds). This will occur even if the data was not collected fully by Tanium.  The default is 30 seconds. |
| pollfreq | The frequency of polling Tanium for more answers. The default is each second. |
| headers | The table's headers to be shown by order. |

## Outputs
---
There are no outputs for this script.
