---
id: account-enrichment-generic-v2.1
title: Account Enrichment Generic V2.1
---

Enriches accounts using one or more integrations.

Supported integrations:
- Active Directory

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

## Sub-playbooks
This playbook does not use any sub-playbooks.

## Integrations
This playbook does not have any integrations.

## Scripts
This playbook does not use any scripts.

## Commands
* ad-get-user

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| Username | The username to enrich. | Username | Account | Optional |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Account | The account object. | unknown |
| ActiveDirectory.Users.sAMAccountName | The user's samAccountName. | unknown |
| ActiveDirectory.Users.userAccountControl | The user's account control flag. | unknown |
| ActiveDirectory.Users.mail | The user's email address. | unknown |
| ActiveDirectory.Users.memberOf | The groups the user is a member of. | unknown |

![Account_Enrichment_Generic_v2.1](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Account_Enrichment_Generic_v2.1.png)
