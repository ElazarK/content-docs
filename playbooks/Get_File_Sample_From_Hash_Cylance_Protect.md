Returns to the war-room a file sample correlating to SHA256  file hashes in the context using Cylance Protect integration.

* SHA256 context path - ${File.SHA256}

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
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
| SHA256 | The SHA256 file hash of the file to download. |  |  | Optional |

## Playbook Outputs
---
There are no outputs for this playbook.

![Get_File_Sample_From_Hash_Cylance_Protect]()
