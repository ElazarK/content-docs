Deprecated. Use the "QRadar Indicator Hunting V2" playbook instead.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
* QRadarFullSearch

### Integrations
This playbook does not use any integrations.

### Scripts
* Set

### Commands
* qradar-get-assets

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| MD5 | The MD5 file hash or an array of hashes to search. |  |  | Optional |
| QradarMD5Field | The MD5 file hash field to search in QRadar. If none are specified, the search will use a payload contains filter. |  |  | Optional |
| SHA1 | The SHA1 file hash or an array of hashes to search. |  |  | Optional |
| QradarSHA1Field | The SHA1 file hash field to search in QRadar. If none are specified, the search will use a payload contains filter. |  |  | Optional |
| SHA256 | The SHA256 file hash or an array of hashes to search. |  |  | Optional |
| QradarSHA256Field | The SHA256 file hash field to search in QRadar. If none are specified, the search will use a payload contains filter. |  |  | Optional |
| IPAddress | The source or destination IP address to search. Can be a single address or an array of addresses. |  |  | Optional |
| QradarIPfield | The IP address field to search in QRadar. If none are specified, the search will use `sourceip` or `destinationip` (combined). | sourceip,destinationip |  | Optional |
| URLDomain | The domain or URL can be single or an array of domain/URLs to search. By default the `LIKE` clause is used. |  |  | Optional |
| URLDomainField | THe URL/Domain field to search in QRadar. If none are specified, the search will use a payload contains filter.  |  |  | Optional |
| SelectFields | The fields to be used in the select. Use comma delimited field names as they appear in AQL. \* is an acceptable value. | * |  | Required |
| TimeFrame | Time frame as used in AQL. For example, "LAST 7 DAYS", "START '2019\-09\-25 15:51' STOP '2019\-09\-25 17:51'". For more examples review IBM's AQL documentation. | LAST 7 DAYS |  | Optional |
| InvestigationFields | The fields to be used for the hunting outputs. These fields are added to the selected field's input. | sourceip,destinationip,username |  | Required |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| QRadar.Search.Result | The Qradar's search results. | string |
| QRadar.DetectedIPs | The IP addresses detected based on `sourceip` and `destinationip` fields in your search. | string |
| QRadar.DetectedUsers | The users detected based on the username field in your search. | string |
| QRadar.DetectedHosts | The hosts detected based on hosts in your assets table. Note that the data accuracy depends on how the asset mapping is configured in QRadar. | string |

![QRadar_Indicator_Hunting](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/QRadar_Indicator_Hunting.png)
