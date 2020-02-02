This playbook is used to block files from running on endpoints. 
This playbook supports the following integrations:
- Palo Alto Networks Traps
- Cybereason
- Carbon Black Enterprise Response
- Cylance Protect v2


## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

## Sub-playbooks
* Block File - Cylance Protect v2
* Block File - Cybereason
* Traps Quarantine Event
* Traps Blacklist File
* Block File - Carbon Black Response

## Integrations
This playbook does not use any integrations.

## Scripts
This playbook does not use any scripts.

## Commands
This playbook does not use any commands.

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| MD5 | The MD5 file hash of the file you want to block. | MD5 | File | Optional |
| SHA256 |  | SHA256 | File | Optional |
| EventId | The tTaps event ID that contains the malicious file to block. |  |  | Optional |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| CbResponse.BlockedHashes.LastBlock.Time | The last block time. | unknown |
| CbResponse.BlockedHashes.LastBlock.Hostname | The last block hostname. | unknown |
| CbResponse.BlockedHashes.LastBlock.CbSensorID | The last block sensor I.D | unknown |

![Block_File_Generic_v2](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Block_File_Generic_v2.png)
