DEPRECATED - Use PAN-OS Commit Configuration instead.
If specified as Panorama, will also push the Policies to the specified Device Group in the instance. (Use `pan-os-commit-configuration` instead)

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
* GenericPolling

### Integrations
This playbook does not use any integrations.

### Scripts
This playbook does not use any scripts.

### Commands
* panorama-push-status
* panorama-push-to-device-group
* panorama-commit-status
* panorama-commit

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| FIrewall_OR_Panorama | Determines if the configured instance is Palo Alto Networks Firewall or Panorama. | Firewall |  | Optional |

## Playbook Outputs
---
There are no outputs for this playbook.

![PanoramaCommitConfiguration](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/PAN-OS_Commit_Configuration.png)
