---
id: pcr-aws-iam-password-policy-misconfig
title: PCR_AWS_IAM_Password_Policy_Misconfig
---

Remediates the following Prisma Cloud AWS IAM password policy alerts.

Prisma Cloud policies remediated:
- AWS IAM password policy allows password reuse
- AWS IAM password policy does not expire in 90 days
- AWS IAM password policy does not have a lowercase character
- AWS IAM password policy does not have a minimum of 14 characters
- AWS IAM password policy does not have a number
- AWS IAM password policy does not have a symbol
- AWS IAM password policy does not have a uppercase character
- AWS IAM password policy does not have password expiration period
- AWS IAM Password policy is insecure

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
This playbook does not use any integrations.

### Scripts
This playbook does not use any scripts.

### Commands
* aws-iam-update-account-password-policy

## Playbook Inputs
---

| **Name** | **Description** | **Required** |
| --- | --- | --- | 
| policyId | Returns the Prisma Cloud policy ID. | Required |

## Playbook Outputs
---
There are no outputs for this playbook.

![PCR_AWS_IAM_Password_Policy_Misconfig](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/PCR_AWS_IAM_Password_Policy_Misconfig.png)
