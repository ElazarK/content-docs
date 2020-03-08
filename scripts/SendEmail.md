---
id: send-email
title: Send Email (Deprecated)
---

`Deprecated`

Use the `send-mail` command instead

Sends an email with the specified parameters.
Attachments are provided as a comma-separated list of entry IDs.
Example usage: `!SendEmail subject="File from war room" body="Please see the attached file. --DBot" to=jane@acme.com cc=john@acme.com attachIDs=89@3,46@3`.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | response, email, server |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* send-mail

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| to | The email addresses for the 'to' field. |
| cc | The email addresses for the 'cc' field. |
| bcc | The email addresses for the 'bcc' field. |
| subject | The subject for the email to be sent. |
| body | The contents (body) of the email to be sent. |
| attachIDs | A comma-separated list of IDs of War Room entries that contain files. This is used to attach files to the outgoing email. For example, "attachIDs=15@8,19@8". |
| htmlBody | Sends an html formatted email. This will override the "body" argument. Both cannot be used. |
| noteEntryID | Sends the textual contents of an entry. |
| replyTo | The address to reply to. |

## Outputs
---
There are no outputs for this script.
