---
id: prisma-cloud-compute-parse-compliance-alert
title: Prisma Cloud Compute Parse Compliance Alert
---

Parses a compliance alert with raw JSON data.


## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python3 |
| Tags | Prisma Cloud Compute |
| Demisto Version | 0.0.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| alert_raw_json | The compliance alert raw JSON. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| PrismaCloudCompute.ComplianceAlert.compliance.description | The compliance description. | String |
| PrismaCloudCompute.ComplianceAlert.compliance.id | The compliance ID. | String |
| PrismaCloudCompute.ComplianceAlert.compliance.type | The compliance type. | String |
| PrismaCloudCompute.ComplianceAlert.time | The compliance alert creation time.| Date |
| PrismaCloudCompute.ComplianceAlert.type | The Entity type. Can be, "host", "image" or "container". | String |
