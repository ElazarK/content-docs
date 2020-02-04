Check for duplicate incidents for the current incident, and close it if any duplicate has been found by machine-learning find duplicates automation.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

## Sub-playbooks
This playbook does not use any sub-playbooks.

## Integrations
This playbook does not use any integrations.

## Scripts
* GetDuplicatesMlv2
* Print
* CloseInvestigationAsDuplicate

## Commands
This playbook does not use any commands.

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| closeThreshold | The candidate with a score above the threshold will close the investigation automatically, and mark it as a duplicate to the current incident. | 0.75 |  | Required |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| foundDuplicates | Whether any duplicate incident were found. | boolean |
| duplicateCandidate | The duplicate top candidate. | unknown |

![DeDup_incidents_ML](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/DeDup_incidents_-_ML.png)
