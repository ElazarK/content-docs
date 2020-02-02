This playbook accepts a file hash and quarantines this file using Traps.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

## Sub-playbooks
* GenericPolling

## Integrations
* Traps

## Scripts
This playbook does not use any scripts.

## Commands
* traps-event-quarantine
* traps-event-quarantine-result

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| EventId | The Traps event ID. The playbook quarantines the related files. |  |  | Optional |

## Playbook Outputs
---
There are no outputs for this playbook.

![Block_File_Quarantine_Traps](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Block_File_Quarantine_Traps.png)
