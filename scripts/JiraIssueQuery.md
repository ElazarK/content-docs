---
id: jira-issue-query
title: Jira Issue Query (Deprecated)
---

`Deprecated`

Queries Jira issues.

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
* jira-issue-query

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| query | The JQL query string. |
| startAt | The index of the first issue to return, where 0-based. (integer) |
| maxResults | The maximum number of issues to return. The default is 50. The maximum allowable value is dictated by the JIRA property `jira.search.views.default.max`. If a value that is higher than this number is specified, the search results will be truncated. |

## Outputs
---
There are no outputs for this script.
