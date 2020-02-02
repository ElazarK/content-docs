The playbook enables you to get all of the corresponding file hashes for a file even if there is only one hash type available.
For example, if we have only the SHA256 hash, the playbook will get the SHA1 and MD5 hashes as long as the
original searched hash is recognized by any our the threat intelligence integrations.


## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

## Sub-playbooks
This playbook does not use any sub-playbooks.

## Integrations
This playbook does not use any integrations.

## Scripts
This playbook does not use any scripts.

## Commands
* file

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| SHA256 | The SHA256 file hash on which to search. | SHA256 | File | Optional |
| SHA1 | The SHA1 file hash on which to search. | SHA1 | File | Optional |
| MD5 | The MD5 file hash on which to search. | MD5 | File | Optional |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| File.SHA256 | The output for detected SHA256 file hash. | string |
| File.SHA1 | The output for detected SHA1 file hash. | string |
| File.MD5 | The output for detected MD5 file hash. | string |

![Convert_file_hash_to_corresponding_hashes](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Convert_file_hash_to_corresponding_hashes.png)
