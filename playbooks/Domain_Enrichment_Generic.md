---
id: domain-enrichment-generic
title: Domain Enrichment Generic
---

Enriches domains using one or more integrations.

Domain enrichment includes:
* Domain reputation
* Threat information

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
* VirusTotal - Private API

### Scripts
* DomainReputation

### Commands
* vt-private-get-domain-report

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| Domain | The domain name to enrich. | Name | Domain | Optional |
| GetReputation | Whether the playbook should get the reputation for the domain. | True | - | Required |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Domain | The domain objects. | unknown |
| DBotScore | The indicator, score, type, and vendor. | unknown |

![Domain_Enrichment_Generic](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Domain_Enrichment_Generic.png)
