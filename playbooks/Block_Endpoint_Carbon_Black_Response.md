Carbon Black Response - isolate an endpoint, given a hostname.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

## Sub-playbooks
This playbook does not use any sub-playbooks.

## Integrations
* carbonblack

## Scripts
This playbook does not use any scripts.

## Commands
* cb-sensor-info
* cb-quarantine-device

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| Hostname | The hostname to isolate. | ${Endpoint.Hostname} |  | Optional |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| CbResponse.Sensors.CbSensorID | The Carbon Black Response Sensors IDs that has been isolated. | unknown |
| Endpoint | The isolated enpoint. | unknown |

![Block_Endpoint_Carbon_Black_Response](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Block_Endpoint_Carbon_Black_Response.png)
