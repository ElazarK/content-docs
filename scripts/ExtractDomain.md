---
id: extract-domain
title: Extract Domain (Deprecated)
---

`Deprecated`

Deprecated - We recommend using `extractIndicators` command instead. 

Extracts Domains from the given text and places them both as output and in the context of a playbook. If an object is given, it will convert it to JSON.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | Utility |
| Demisto Version | 0.0.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| text | The text to extract domains from. If the object will convert to JSON. |
| urlRegex | The regex to recognize URLs. |
| markAsIndicator | Creates a new indicator for each new domain found. The default is "true". |
| calcReputation | Whether to calculate the reputation for the new indicator created or not to. The default is "true". |
| tldList | The name of the Demisto list to hold the known TLD list. This will be ignored when looking for domains. |
| extractFromEmails | Fetches the domains from the emails found in a given text. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Domain.Name | The extracted domains. | Unknown |
