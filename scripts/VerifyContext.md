---
id: verify-context
title: Verify Context
---

`Deprecated`

Deprecated, use playbook filters instead.

Verifies path in context:
- Verifies the paths existence
- If the matching object is an array, it will verify that the fields exist in each of the objects in the array.
- If the matching object is not an array, it will verify that the fields exist in the matching object.
- If the 'expectedValue' is given, it will ensure that the given value is equal to the context path.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | javascript |
| Tags | context, Utility |
| Demisto Version | 0.0.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| path | The context path. For example, "Incidents". |
| fields | The comma-separated values to verify that are in context. For example, "one,two,three". |
| expectedValue | The Primitive or JSON expected value of the path context. For example, ""SomeString", "{"a": 1, "b": ["hello", "world" ]}". |

## Outputs
---
There are no outputs for this script.
