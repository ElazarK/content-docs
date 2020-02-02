This playbook investigates an access incident by gathering user and IP information.
The playbook then interacts with the user that triggered the incident to confirm whether or not they initiated the access action.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

## Sub-playbooks
* Account Enrichment - Generic
* IP Enrichment - Generic

## Integrations
* Builtin

## Scripts
* AssignAnalystToIncident
* EmailAskUser
* ADGetUser

## Commands
* setIncident
* closeInvestigation

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| SrcIP | The source IP address from which the incident originated. | src | incident | Optional |
| DstIP | The target IP address that was accessed. | dest | incident | Optional |
| Username | The username of the account that was used to access the DstIP. | srcuser | incident | Optional |
| Role | The default role to assign the incident to. | Administrator |  | Required |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Account.Email.Address | The email address object associated with the account. | string |
| DBotScore | The indicator, score, type, and vendor. | unknown |
| Account.ID | The unique account DN \(Distinguished Name\). | string |
| Account.Username | The account username. | string |
| Account.Email | The email address associated with the Account. | unknown |
| Account.Type | Type of the Account entity. | string |
| Account.Groups | The groups the Account is part of. | unknown |
| Account | Account object. | unknown |
| Account.DisplayName | The Account display name. | string |
| Account.Manager | The Account's manager. | string |
| DBotScore.Indicator | The indicator value. | string |
| DBotScore.Type | The indicator's type. | string |
| DBotScore.Vendor | The indicator's vendor. | string |
| DBotScore.Score | The indicator's score. | number |
| IP | The IP address objects. | unknown |
| Endpoint | The Endpoint's object. | unknown |
| Endpoint.Hostname | The hostname to enrich. | string |
| Endpoint.OS | The endpoint OS. | string |
| Endpoint.IP | The list of endpoint IP addresses. | unknown |
| Endpoint.MAC | The list of endpoint MAC addresses. | unknown |
| Endpoint.Domain | The endpoint domain name. | string |

![Access_Investigation_Generic](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Access_Investigation_Generic.png)
