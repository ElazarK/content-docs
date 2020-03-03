---
id: qradar-classifier
title: QRadar Classifier (Deprecated)
---

`Deprecated`

This script Classifies QRadar incidents. The `QRADAR_CATEGORIES` dictionary translate QRadar `High level Categories` to its `Demisto Types` counterpart.

For custom categories, use the `customCategories` argument. The offense high level category will be put to context. 

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | QRadar, Classifier |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* qradar-searches

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| customCategories | The option to add custom categories to the classifier. JSON with QRadar high level category and their Demisto type counterparts. For example, "{"QRadarCategory1" : "DemistoType1", "QRadarCategory2" : "DemistoType2"}".  |
| contextOutput | The high level category output. The default is set to "Classifier/Description". |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Classifier/Description | The QRadar offense `High level category`. | Unknown |
