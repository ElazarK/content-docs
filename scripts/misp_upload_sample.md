---
id: misp-upload-sample
title: MISP Upload Sample (Deprecated)
---

`Deprecated`

Uploads a malicious file sample to MISP.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags |  |
| Demisto Version | 0.0.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| fileEntryID | The entry ID of the file to upload. |
| event_id | The event's ID is optional. It can be either supplied via the URL or the posted object. The URL has priority if both are provided. Not supplying an event ID will cause MISP to create a single new event for all of the posted malware samples. You can define the default settings for the event, otherwise a set of default settings will be used. |
| distribution | The distribution setting used for the attributes and for the newly created event, if relevant. [0-3] |
| to_ids | The attributes flagged and created during the transaction to be marked as `to_ids` or not. |
| category | The category that will be assigned to the uploaded samples. Can be, "Payload delivery", "Artifacts dropped", "Payload Installation", or "External Analysis". |
| info | The event info field to be populated if no event ID was supplied. Alternatively, if this is not set, MISP will generate a message showing that it's a malware sample collection generated on the given day. |
| analysis | The analysis level of the newly created event, if applicable. [0-2] threat_level_id: The threat level ID of the newly created event, if applicatble. [0-3] |
