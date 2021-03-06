---
id: email-address-enrichment-generic-v2
title: Email Address Enrichment Generic V2
---

Enriches email addresses.  

Email address enrichment involves:
- Getting information from Active Directory for internal addresses.
- Getting the domain-squatting reputation for external addresses.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
This playbook does not use any integrations.

### Scripts
* Exists
* IsEmailAddressInternal
* ADGetUser
* EmailDomainSquattingReputation

### Commands
This playbook does not use any commands.

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| InternalDomains | The CSV list of internal domains. The list will be used to determine whether an email address is internal or external. | None | inputs.InternalDomains | Optional |
| Email | The email addresses to enrich. | Email.Address | Account | Optional |
| Domain | The domains associated with the incident. | inputs.Domain | - | Optional |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Account | The account object. | unknown |
| Account.Email.Address | The email account full address. | string |
| Account.Groups | The groups the account belongs to. | string |
| Account.Email.Domain | The email account domain. | string |
| Account.Email.NetworkType | The email account networktype. Can be, "Internal" or "External". | string |
| Account.Type | The account entity type. | string |
| Account.Email.Username | The email account username. | string |
| Account.ID | The unique account DN (Distinguished Name). | string |
| Account.DisplayName | The account display name. | string |
| Account.Manager | The account's manager. | string |
| Account.Email.Distance.Domain | The compared domain. | string |
| Account.Email.Distance.Value | The distance between the email domain and the compared domain.  | number |
| DBotScore.Indicator | The indicator. | string |
| DBotScore | The DBotScore object. | unknown |
| DBotScore.Type | The indicator type. | string |
| DBotScore.Vendor | The DBot score vendor. | string |
| DBotScore.Score | The DBot score. | number |

![Email_Address_Enrichment_Generic_v2](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Email_Address_Enrichment_Generic_v2.png)
