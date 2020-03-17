---
id: misp-download-sample
title: MISP Download Sample (Deprecated)
---

`Deprecated`

Downloads the malicious file sample from MISP.

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
| hash | The hash in MD5 format. If `allSamples` is set, then this can be be, "md5", "sha1", or "sha256". |
| eventID | Will only fetch data from the given event ID if set. |
| allSamples | Will return all samples from events that have a match for the hash provided above, if set. |

## Outputs
---
There are no outputs for this script.
