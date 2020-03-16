---
id: google-apps-gmail-search
title: Google Apps Gmail Search (Deprecated)
---

`Deprecated`

Searches for the messages in the user's mailbox.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | google apps |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* googleapps-gmail-search

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| userKey | Identifies the user in the API request. Can be, the user's, "primary email address", "alias email address", or "a unique user ID". |
| query | Returns messages that match the specified query. This supports the same query format as the Gmail search box. For example, "from:someuser<span>@example.com rfc822msgid: is:unread". For syntex click [here]("https://support.google.com/mail/answer/7190?hl=en"). |
| maxResults | The maximum number of results to return. The default is 100. The maximum is 500. The acceptable values are, 1 to 500, inclusive. |
| fields | The partial responses allowed by the field to be retrieved. Click [here](https://developers.google.com/gdata/docs/2.0/basics#PartialResponse) for more information. (comma-separated list) |
| labelsIds | The messages only to return with labels that match all of the specified label IDs. (comma-separated list) |
| pageToken | The page token to retrieve a specific page of results from within the list. |
| includeSpamTrash | The messages to include from `SPAM` and `TRASH` in the results. The default is "false". |

## Outputs
---
There are no outputs for this script.
