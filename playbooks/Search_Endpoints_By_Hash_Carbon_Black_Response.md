---
id: search-endpoints-by-hash-carbon-black-response
title: Search Endpoints by Hash Carbon Black Response
---

Hunts for malicious indicators using Carbon Black.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
This playbook does not use any integrations.

### Scripts
* CBFindHash
* Set

### Commands
This playbook does not use any commands.

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| Hash | The MD5 file hash. | MD5 | File | Optional |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Endpoint.Hostname | The device hostname. | string |
| Endpoint | The endpoint. | unknown |

![Search_Endpoints_By_Hash_Carbon_Black_Response](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Search_Endpoints_By_Hash_Carbon_Black_Response.png)
