Lists NetWitness SA incidents. Filtering and sorting the list is also supported (see optional arguments).

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | RSA NetWitness Security Analytics |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* nw-list-incidents

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| query | Whether the query provided all other ignored parameters. The query should contain page, limit, start, sort and filter, joined by "&". For example, "page=1&start=0&limit=100&sort=[{"property":"created","direction":"DESC"}]&filter=[{"property":"created","value":[851171984031,1482323984031]}]". |
| page | Indicates the number of pages of the incident. The default is 1.  |
| start | Indicates the starting index of the incident in the page. The default is 0.  |
| limit | Limits the number of incidents per page. The default is 100. |
| sort | Sorts by "created" field in "DESC" order. This is the default method. For example, "[{"property":"created","direction":"DESC"}]". |
| filter | Filters by "created" from 1996 to this date. This is the default method. For example, "[{"property":"id", "value":"INC-21"}]". |
| incidentManagementId | The ID of the NetWitness INCIDENT_MANAGEMENT device/component ID. This can be received by running the `nw-get-component` command. If this argument is not filled/passed, the script will automatically get the first device of type INCIDENT_MANAGEMENT from the SA server. [optional number] |

## Outputs
---
There are no outputs for this script.
