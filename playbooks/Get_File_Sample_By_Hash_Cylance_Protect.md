---
id: get-file-sample-by-hash-cylance-protect
title: Get File Sample by Hash Cylance Protect
---

Returns to the War Room, a file sample correlating to SHA256 hashes in the inputs using Cylance Protect integration.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
* Cylance Protect v2
* Cylance Protect

### Scripts
* UnzipFile
* Exists
* http

### Commands
* cylance-protect-download-threat

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| SHA256 | The SHA256 hash of the file to download. | SHA256 | File | Optional |
| ZipPassword | The password for the zip file. | infected | - | Required |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| File | The sample file. | unknown |


![Get_File_Sample_By_Hash_Cylance_Protect](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Get_File_Sample_By_Hash_Cylance_Protect.png)
