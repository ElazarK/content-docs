---
id: prisma-cloud-compute-parse-cloud-discovery-alert
title: Prisma Cloud Compute Parse Cloud Discovery Alert
---

Parses cloud discovery alerts with raw JSON data.

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
| PrismaCloudCompute.CloudDiscoveryAlert.time | The alert creation timestamp. | Date |
| PrismaCloudCompute.CloudDiscoveryAlert.credentialId | The ID reference of the credential used. | String |
| PrismaCloudCompute.CloudDiscoveryAlert.provider | The cloud provider. For example, "AWS", or "GCP". | String |
| PrismaCloudCompute.CloudDiscoveryAlert.serviceType | The cloud service type. For example, "ECR", or "GCR". | String |
| PrismaCloudCompute.CloudDiscoveryAlert.region | The region that was scanned. For example, GCP - "us-east-1", Azure - "westus". | String |
| PrismaCloudCompute.CloudDiscoveryAlert.project | The GCP project that was scanned. | String |
| PrismaCloudCompute.CloudDiscoveryAlert.registry | The Azure registry that was scanned. For example, `testcloudscanregistry.azurecr.io`. | String |
| PrismaCloudCompute.CloudDiscoveryAlert.protected | The number of protected entities. For example, "registries", "functions", or "clusters". | Number |
| PrismaCloudCompute.CloudDiscoveryAlert.total | The total number of entities found in cloud scan. | Number |
| PrismaCloudCompute.CloudDiscoveryAlert.err | Holds any error found during a scan. | String |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.name | The name of the entity. | String |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.protected | Whether the entity is protected. | Number |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.lastModified | The modification time of the function. | Date |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.runtime | The runtime environment for the function. For excample, "nodejs". | String |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.version | The version of the entity. | String |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.arn | The Amazon Resource Name (ARN) assigned to the entity. | String |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.status | The current status of entity. | String |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.runningTasksCount | The number of running tasks in ECS cluster. | Number |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.activeServicesCount | The number of active services in ECS cluster. | Number |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.createdAt | The time when the entity was created. | Date |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.nodesCount | The number of nodes in the cluster. For example, "aks" or "gke". | Number |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.resourceGroup | The the Azure resource group containing the entity. | String |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.containerGroup | The Azure ACI container group the container belongs to. | String |
| PrismaCloudCompute.CloudDiscoveryAlert.entities.image | The image of the ACI container. | String |
| PrismaCloudCompute.CloudDiscoveryAlert.collections | The matched result collections. | String |
| PrismaCloudCompute.CloudDiscoveryAlert.accountID | The cloud account ID. | Date |
