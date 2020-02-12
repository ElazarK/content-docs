This playbook accepts a SHA256 file hash and adds it to a blacklist using Traps integration.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
This playbook does not use any integrations.

### Scripts
This playbook does not use any scripts.

### Commands
* traps-hash-blacklist

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| SHA256 | The Malicious SHA256 file hash. | SHA256 | File | Optional |

## Playbook Outputs
---
There are no outputs for this playbook.

![Traps_Blacklist_File](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Traps_Blacklist_File.png)
