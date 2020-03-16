---
id: google-apps-list-users
title: Google Apps List Users (Deprecated)
---

`Deprecated`

Retrieves a paginated list of either deleted users or all users in a domain.

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
* googleapps-list-users

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| domain | The domain name used to get the fields from only one domain. To return all domains for a customer account, use the customer query parameter instead. Either the customer or the domain parameter must be provided. |
| customer | The unique ID for the customer's Google account. By default, this will use the value in the integration page. In the case of a multi-domain account, to fetch all groups for a customer, fill this field instead of the domain field. An account administrator, can also use the `my_customer` alias to represent the accounts `customerId`. The `customerId` is also returned as part of the user's resource. Either the customer or the domain parameter must be provided. |
| viewTypePublicDomain | Whether to fetch the administrator-only or domain-wide public view of the user. This will use `admin_view`, which the results include both administrator-only and domain-public fields for the user. The default is "admin_view". If true it will use "domain_public", the results only include fields for the user that are publicly visible to other users in the domain. |
| maxResults | The maximum number of results to return. The default is 100. The maximum is 500. The acceptable values are 1 to 500, inclusive. |
| customFieldMask | The comma-separated list of schema names. All fields from these schemas are fetched. This should only be set when "projection=custom". |
| event | The event sets the optional parameter "event", which means the event on which subscription is intended (if subscribing). Can be, "add", "delete", "makeAdmin", "undelete", or "update". |
| query | The query string search. This should be of the form "". For the complete documentation click [here](https://developers.google.com/admin-sdk/directory/v1/guides/search-users). |
| projection | The subset of fields to fetch for this user. Can be, "basic" which means to not include any custom fields for the user. This is the default. "custom" which include custom fields from schemas requested in `customFieldMask`. "full" which include all fields associated with this user. |
| showDeleted | The list of deleted users to retrieve when set to "true". The default is "false". |
| sortOrder | The results to be returned in ascending or descending order. Can be, "ASCENDING" or "DESCENDING". |

## Outputs
---
There are no outputs for this script.
