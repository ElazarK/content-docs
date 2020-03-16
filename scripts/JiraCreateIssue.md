---
id: design-best-practices
title: Integration Design Best Practices  (Deprecated)
---

`Deprecated`

Creates a new issue on Jira.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | jira |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* jira-create-issue

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| issueJson | The issue object in JSON format. |
| summary | The summary of the issue. This is a mandatory field. |
| projectKey | The project key to associate the issue. |
| issueTypeName | The issue type name. For example, "Incident". |
| issueTypeId | The issue type ID. (number) |
| projectName | The project name to associate the issue with. |
| description | The issue's description. |
| labels | The comma-separated list of labels.  |
| priority | The priorty name. For example, "High" or "Medium". |
| dueDate | The due date for the issue. It should be in format of 2018-03-11. |
| assignee | The assignee name. |
| reporter | The reporter name. |

## Outputs
---
There are no outputs for this script.
