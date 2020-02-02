Enrich Accounts using one or more integrations

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

## Sub-playbooks
This playbook does not use any sub-playbooks.

## Integrations
This playbook has no integrations.

## Scripts
* ADGetUser
* Exists

## Commands
* ad-get-user

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| Username | The Username to enrich | ${Account.Username} |  | Optional |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Account | The account object. | unknown |
| Account.Type | The type of the account entity. | string |
| Account.ID | The unique account DN \(Distinguished Name\). | string |
| Account.Username | The account username. | string |
| Account.Email | The email address associated with the account. | unknown |
| Account.Groups | The groups the account is part of. | unknown |
| Account.DisplayName | The account display name. | string |
| Account.Manager | The account's manager. | string |

![Account_Enrichment_Generic](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Account_Enrichment_Generic.png)
