---
id: get-ml-features
title: Get Ml Features
---

Calculates features for machine learning.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | ml |
| Demisto Version | 3.5.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| maxNumberOfIncidents | The maximum number of incidents to check. |
| anonymousData | Whether the incident data should be anonymous. |
| uploadToS3 | Uploads the data to s3. |
| awsInfo | The comma-separated values, "AWS_ACCESS_KEY,AWS_SECRET_KEY,AWS_BUCKET,AWS_CLIENT_ID". |
| incidentsQuery | The query used to fetch incidents from the database. |
| recursive_related | Checks for second degree related incidents. |

## Outputs
---
There are no outputs for this script.
