Collects data using McAfee Active Response, from an endpoint for IR purposes (requires ePO as well).

Input:
* Hostname (Default: ${Endpoint.Hostname})

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
* McAfee Active Response

### Scripts
* Exists
* EPOFindSystem

### Commands
* mar-search-multiple

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Required** |
| --- | --- | --- | --- |
| Hostname | The hostname to run on. | ${Endpoint.Hostname} | Optional |

## Playbook Outputs
---
There are no outputs for this playbook.

![MAR_Endpoint_data_collection](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/MAR_Endpoint_data_collection.png)
