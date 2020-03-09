---
id: slack-mirror
title: Slack Mirror (Deprecated)
---

`Deprecated`

Mirrors an incident to a Slack private channel. You can chose what to mirror with the type argument. A Slack private channel will be created and the incident team invited. Messages on Slack will be reflected in the War Room and vice versa.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | slack |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* slack-mirror-investigation

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| type | The type of mirroring can be set to, "all" to mirror everything, "chat" to mirror only chatting but not commands, or "none" to stop mirroring. |

## Outputs
---
There are no outputs for this script.
