---
id: search-incidents
title: Search Incidents
---

`Deprecated` 

Use `SearchIncidents` instead.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | Utility |
| Demisto Version | 0.0.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| id | The incident IDs by which to filter. |
| name | The incident name by which to filter. |
| status | The status by which to filter. For example, "assigned". |
| notstatus | The excluding status by which to filter. For example, "assigned". |
| reason | The closing reason by which to filter. |
| fromdate | The from date by which to filter. For example, "2006-01-02T15:04:05+07:00" or "2006-01-02T15:04:05Z". |
| todate | The date by which to filter. For example, "2006-01-02T15:04:05+07:00" or "2006-01-02T15:04:05Z". |
| fromclosedate | The from close date by which to filter. For example, "2006-01-02T15:04:05+07:00" or "2006-01-02T15:04:05Z". |
| toclosedate | The to close date by which to filter. For example, "2006-01-02T15:04:05+07:00" or "2006-01-02T15:04:05Z". |
| fromduedate | The from due date by which to filter. For example, "2006-01-02T15:04:05+07:00" or "2006-01-02T15:04:05Z". |
| toduedate | The to due date by which to filter. For example, "2006-01-02T15:04:05+07:00" or "2006-01-02T15:04:05Z". |
| level | The severity by which to filter. |
| owner | The incident owners by which to filter. |
| details | The incident details by which to filter. |
| type | The incident type by which to filter. |
| query | The free form query (use Lucene syntax) by which to filter. All other filters will be ignored if this filter is used. |
| page | The page number by which to filter. |
| size | The page size by which to filter (per fetch). |
| sort | The format to sort by. For example, "field.asc,field.desc,...". |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| foundIncidents.id | The IDs of the found incidents. | Unknown |
| foundIncidents.name | The names of the found incidents. | Unknown |
| foundIncidents.severity | The severities of the found incidents. | Unknown |
| foundIncidents.status | The statuses of the found incidents. | Unknown |
| foundIncidents.owner | The owners of the found incidents. | Unknown |
| foundIncidents.created | The create dates of the found incidents. | Unknown |
| foundIncidents.closed | The close dates of the found incidents. | Unknown |
| foundIncidents.labels | The array of labels per incident of the found incidents. | Unknown |
| foundIncidents.details | The details of the found incidents. | Unknown |
| foundIncidents.dueDate | The due dates of the found incidents. | Unknown |
| foundIncidents.phase | The phases of the found incidents | Unknown |
