Deprecated: We recommend using extractIndicators command instead.
Extract indicators from input data.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
This playbook does not use any integrations.

### Scripts
* ExtractDomain
* ExtractEmail
* ExtractURL
* ExtractHash
* ExtractIP

### Commands
This playbook does not use any commands.

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| incident | The incident used the integration.  | ${incident} |  | Optional |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| File.MD5 | The extracted MD5 file hash. | string |
| File.SHA1 | The extracted SHA1 file hash. | string |
| File.SHA256 | The extracted SHA256 file hash. | string |
| URL.Data | The extracted URLs. | string |
| IP.Address | The extracted IP addresses. | string |
| Domain.Name | The extracted domains. | string |
| Account.Email.Address | The extracted emails.| string |

![Extract_Indicators_Generic](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Extract_Indicators_Generic.png)