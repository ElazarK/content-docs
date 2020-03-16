---
id: google-apps-gmail-get-mail
title: Google Apps Gmail Get Mail (Deprecated)
---

`Deprecated`
Gets the specified message.
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
* googleapps-gmail-get-mail

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| userKey | The identifier used for the user in the API request. Can be, the user's "primary email address", "alias email address", or "a unique user ID". |
| messageId | The ID of the message to retrieve. |
| fields | The fields allows partial responses to be retrieved. Click [here](https://developers.google.com/gdata/docs/2.0/basics#PartialResponse) for more information. (comma-separated) |
| format | The format to return the message in. Can be, "full", which returns the full email message data with its body content parsed in the payload field. The raw field is not used. (default) "Metadata", which returns only the email message ID, labels, and email headers. "Minimal", which Returns only email message ID and labels. This does not return the email headers, body, or payload. "Raw" which returns the full email message data with body content in the raw field as a Base64URL encoded string. The payload field is not used. The default is "full".  |

## Outputs
---
There are no outputs for this script.
