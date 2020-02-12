Collect endpoint information based on SentinelOne commands.

Input:
* Hostname (Default: ${Endpoint.Hostname})

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
* SentinelOne

### Scripts
* Print
* Exists

### Commands
* so-agents-query
* so-get-agent-processes

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| Hostname | The hostname of the device to run on. | ${Endpoint.Hostname} |  | Optional |

## Playbook Outputs
---
There are no outputs for this playbook.
![Sentinel_One_Endpoint_data_collection](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Sentinel_One_Endpoint_data_collection.png)
