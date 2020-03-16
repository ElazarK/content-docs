---
id: google-apps-get-user
title: Google Apps Get User (Deprecated)
---

`Deprecated`

Fetches information on a specific user.

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
* googleapps-get-user

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| userKey | Identifies the user in the API request. Can be, the user's, "primary email address", "alias email address", or "a unique user ID". |
| projection | The subset of fields to fetch for the user. Can be, "basic" which does not include any custom fields for the user, "custom" which includes custom fields from schemas requested in `customFieldMask`, "full" which include all fields associated with this user. The default is "basic". |
| viewTypePublicDomain | Whether to fetch the administrator-only or domain-wide public view of the user. The default is "`admin_view`". The results include both administrator-only and domain-public fields for the user. If this is set to "true" it will use "domain_public", which the results only include fields for the user that are publicly visible to other users in the domain. |
| customFieldMask | The comma-separated list of schema names. All fields from these schemas are fetched. This should only be set when `projection=custom`. |

## Outputs
---
There are no outputs for this script.
