This playbook returns a file sample to the war-room given the file's SHA256 file hash, using Cylance Protect v2 integration.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
* Cylance Protect v2

### Scripts
This playbook does not use any scripts.

### Commands
* cylance-protect-download-threat

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| SHA256 | The SHA256 file hash of the file. | SHA256 | File | Optional |
| unzip | Specifies whether the downloaded file will be unzipped. The default is 'no'. Yes will unzip automatically
No will not unzip automatically. |  |  | Optional |

## Playbook Outputs
---
There are no outputs for this playbook.

![Get_File_Sample_By_Hash_Cylance_Protect_v2](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Get_File_Sample_By_Hash_Cylance_Protect_v2.png)
