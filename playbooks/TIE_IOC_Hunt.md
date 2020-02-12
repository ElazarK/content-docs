Hunt for sightings of MD5 file hash, SHA1 file hash and/or SHA256 file hashes on endpoints, using McAfee TIE (requires ePO as well).

Input:
* Hash (default, takes all deferent hashes from context)

Output:
* All agents that files with "Hash" has been executed on (TIE)
* Enrich Agents info from ePO

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
* McAfee Threat Intelligence Exchange

### Scripts
* EPOFindSystem
* Exists

### Commands
* tie-file-references

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| Hash | The hash to hunt. Can be, "MD5", "SHA1", or "SHA256". The default is set to all hashes | ${.=val.File.map(function(f) {return [f.MD5, f.SHA1, f.SHA256];}).reduce(function(a, b){return a.concat(b);}, []).filter(function (val1) {return val1;})} |  | Optional |

## Playbook Outputs
---
There are no outputs for this playbook.
![TIE_IOC_Hunt](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/TIE_IOC_Hunt.png)
