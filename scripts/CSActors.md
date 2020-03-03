---
id: cs-actors
title: CS Actors (Deprecated)
---

`Deprecated`

Queries CrowdStrike actors based on the given parameters. Fields such as countries and industries, which can contain multiple values, can be passed separated by ','.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | server, threat-intel, crowdstrike |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* cs-actors

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| q | Searches all fields for the given data. |
| name | Searches based on the actor name. |
| description | Searches based on the description. |
| minLastModifiedDate | Searches a range from the modified date. Dates are formatted as YYYY-MM-DD. |
| maxLastModifiedDate | Searches a range to the modified date. Dates are formatted as YYYY-MM-DD. |
| minLastActivityDate | Searches a range from the activity date. Dates are formatted as YYYY-MM-DD. |
| maxLastActivityDate | Searches a range to the activity date. Dates are formatted as YYYY-MM-DD. |
| origins | Searches by origins. This will accept a comma-separated list. |
| targetCountries | Searches by target countries. This will accept a comma-separated list. |
| targetIndustries | Searches by target industries. This will accept a comma-separated list. |
| motivations | Searches by motivations. This will accept a comma-separated list. |
| sort | Sorts by `field_name.order`. `field_name.order` where order is either ascend or descend. |
| offset | The page number of the results to retrieve. It is 0 based. |
| limit | The number of results for each page. |

## Outputs
---
There are no outputs for this script.
