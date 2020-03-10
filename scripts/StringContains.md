---
id: string-contains
title: String Contains (Deprecated)
---

`Deprecated`

This script is deprecated. Please use the `StringContainsArray` filter which implements the same functionality.

Checks whether a substring is within string. 

It will return:
yes - string contains substring.
no - string does not contain substring.

If the `stringSeperator` is provided, the substring will be split using the separator, and each item will be checked.
If one of the items is found in the string, the script returns "yes".

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | Condition, Utility |
| Demisto Version | 0.0.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| string | The string to check (haystack). |
| substring | The string that will be searched for within the string argument (needle). |
| substringSeperator | The seperator for splitting the substring (needle) and the search for each item. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| True | Wether the string contains a substring. | Unknown |
| False | Wether the string does not contain substring. | Unknown |
