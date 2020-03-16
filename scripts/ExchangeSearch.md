---
id: exchange-search
title: Exchange Search (Deprecated)
---

`Deprecated`

Searches mails on the Exchange Web Server (EWS).

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | ews, exchange, server, email |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* ews-search-mailbox

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| mailbox | The mailbox to be searched. For example, "dave<span>@acme.com". |
| subject | Only matches mails containing a specific subject. |
| attachmentName | Only matches mails containing an attachment with a specific name. |
| sender | Only matches mails from a specific sender (Email address). |
| body | Only matches mails containing a specific body. |

## Outputs
---
There are no outputs for this script.
