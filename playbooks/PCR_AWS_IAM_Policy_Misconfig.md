---
id: pcr-aws-iam-policy-misconfig
title: PCR AWS IAM Policy Misconfig
---

Remediates Prisma Cloud AWS IAM policy alerts.  It uses sub-playbooks that perform the remediation steps.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
* Prisma Cloud Remediation - AWS IAM Password Policy Misconfiguration

### Integrations
* RedLock
* Builtin

### Scripts
This playbook does not use any scripts.

### Commands
* closeInvestigation
* aws-iam-get-account-password-policy
* redlock-dismiss-alerts

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| AutoUpdatePasswordPolicy | Whether to update AWS IAM password policy automatically. | no | - | Optional |
| policyId | Returns the Prisma Cloud policy ID. | labels.policy | incident | Optional |

## Playbook Outputs
---
There are no outputs for this playbook.

![PCR_AWS_IAM_Policy_Misconfig](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/PCR_AWS_IAM_Policy_Misconfig.png)
