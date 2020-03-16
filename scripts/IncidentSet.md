---
id: incident-set
title: Incident Set (Deprecated)
---

`Deprecated`

Modifies the incident information, such as name, owner, type, etc.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | management |
| Demisto Version | 3.5.1 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| owner | The incident owner. Must be, an existing user in the platform. |
| playbook | The assigned new playbook name. |
| stage | The incident stage. Must be, from a predefined list of stages |
| details | The incident's details. |
| severity | The severity to set. Can be, "unknown", "low", "medium", "high" or "critical". |
| type | The incident type. |
| name | The incident name. |
| updatePlaybookForType | Whether to update the playbook according to the new given type. Can be, "yes" or "no". The default is "yes". |
| labels | Sets and overrides the labels for the incident. The label's expected format is "[{"labelName": "labelValue"}, {"labelName1": "labelValue1"}]" (JSON). |
| addLabels | The list of labels to add to for the incident. The label's expected format is "[{"labelName": "labelValue"}, {"labelName1": "labelValue1"}]" (JSON). |
| customFieldName | The name of the custom field you want to change. |
| customFieldValue | The value to set for the field specified in `customFieldName`. |

## Outputs
---
There are no outputs for this script.
