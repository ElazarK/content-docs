---
id: netwitness-search
title: Netwitness Search
---

Searches for matches in a session or packet's content.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | RSA NetWitness Packets & Logs |
| Demisto Version | 0.0.0 |

## Dependencies
---
This script uses the following commands and scripts.
* nw-sdk-search

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| session | The session ID to search. (uint64) |
| size |  The maximum number of entries to return. (uint32, {range:1 to 1677721}) |
| search | The search string to use. (string) |

## Outputs
---
There are no outputs for this script.
