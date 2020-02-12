Parse Audit alert raw JSON data
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
| alert_raw_json | The compliance alert raw JSON |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| PrismaCloudCompute.AuditAlert.activityType | The type of the activity. | String |
| PrismaCloudCompute.AuditAlert.appID | The RASP application ID. | String |
| PrismaCloudCompute.AuditAlert.category | The audit category. | String |
| PrismaCloudCompute.AuditAlert.command | The original command (with arguments) the user invoked. | String |
| PrismaCloudCompute.AuditAlert.container | The container name in which the alert occurred. | String |
| PrismaCloudCompute.AuditAlert.forensicLink | The link for downloading the forensic data for the related incident. | String |
| PrismaCloudCompute.AuditAlert.fqdn | The FQDN of the host in which the alert occurred. | String |
| PrismaCloudCompute.AuditAlert.function | The name of the serverless function which triggered the alert. | String |
| PrismaCloudCompute.AuditAlert.host | The host name in which the alert occurred. | String |
| PrismaCloudCompute.AuditAlert.image |The image name in which the alert occurred. | String |
| PrismaCloudCompute.AuditAlert.interactive | Whether the alert belongs to an interactive session. | Boolean |
| PrismaCloudCompute.AuditAlert.kubernetesResource | The resource name in which the alert occurred. | String |
| PrismaCloudCompute.AuditAlert.line | The matching log line. | String |
| PrismaCloudCompute.AuditAlert.logfile | The log file which was inspected. | String |
| PrismaCloudCompute.AuditAlert.message | The audit message. | String |
| PrismaCloudCompute.AuditAlert.region | The region of the serverless function. | String |
| PrismaCloudCompute.AuditAlert.rule | The rule which triggered the alert. | String |
| PrismaCloudCompute.AuditAlert.runtime | The language runtime of the serverless function. | String |
| PrismaCloudCompute.AuditAlert.service | The owning systemd service. | String |
| PrismaCloudCompute.AuditAlert.time | The time when the alert occurred. | Date |
| PrismaCloudCompute.AuditAlert.type | The type of the audit alert. | String |
| PrismaCloudCompute.AuditAlert.user | The user initiated the alert. | String |
