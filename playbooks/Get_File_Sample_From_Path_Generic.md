Returns a file sample to the war-room from a path on an endpoint using one or more integrations.

inputs:
* UseD2 - If "True", use the Demisto Dissolvable Agent (D2) to return the file. The default is "False".

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
* Get File Sample From Path - Carbon Black Enterprise Response
* Get File Sample From Path - D2

### Integrations
This playbook does not use any integrations.

### Scripts
This playbook does not use any scripts.

### Commands
This playbook does not use any commands.

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| UseD2 |  | no |  | Optional |
| Hostname | The endpoint hostname.  | ${Endpoint.Hostname} |  | Optional |
| Path | The path of the file. | ${File.Path} |  | Optional |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| File | The file to sample. | unknown |

![Get_File_Sample_From_Path_Generic](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Get_File_Sample_From_Path_Generic.png)