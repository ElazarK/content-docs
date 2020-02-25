`Deprecated` We recommend using Phishing investigation - Generic playbook instead.  

Investigates suspected Phishing attempts. This is an automated playbook.
It picks up the required information from the incident metadata as created by the mail listener.

Labels:
- Email/from: The email address of the user targeted by the suspected phishing attempt, who reported the email by forwarding it.
- Email: The to recipients.
- Email/cc: The cc recipients.
- Email/format: The format of the email - text / html / etc.
- Email/html: The html body.
- Email/text: The text body.
- Email/subject: The subject of the email.
- Email/attachments: The list of attachments.
- Email/headers: The headers for the email.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
This playbook does not use any integrations.

### Scripts
* Exists
* Set
* IsMaliciousIndicatorFound
* ExtractURL
* CheckSenderDomainDistance
* ExtractIP
* SendEmail
* CloseInvestigation

### Commands
This playbook does not use any commands.

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Required** |
| --- | --- | --- | --- | 
| CompanyDomains | The domains for the company to try and match closeness of sender. (comma-separated) | company.com | Optional |

## Playbook Outputs
---
There are no outputs for this playbook. 

![PhishingAutomated](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/PhishingAutomated.png)
