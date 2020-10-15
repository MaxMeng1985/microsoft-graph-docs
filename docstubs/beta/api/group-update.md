---
title: "Update group"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update group

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a group object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Request headers

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request Body

In the request body, supply JSON representation of the [group](../resources/-group.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a group object.

| Property                      | Type                                                                                  | Description |
| :---------------------------- | :------------------------------------------------------------------------------------ | :---------- |
| assignedLabels                | [assignedLabel](../resources/assignedlabel.md) collection                             |             |
| assignedLicenses              | [assignedLicense](../resources/assignedlicense.md) collection                         |             |
| classification                | String                                                                                |             |
| createdByAppId                | String                                                                                |             |
| createdDateTime               | DateTimeOffset                                                                        |             |
| description                   | String                                                                                |             |
| displayName                   | String                                                                                |             |
| expirationDateTime            | DateTimeOffset                                                                        |             |
| groupTypes                    | String collection                                                                     |             |
| hasMembersWithLicenseErrors   | Boolean                                                                               |             |
| infoCatalogs                  | String collection                                                                     |             |
| isAssignableToRole            | Boolean                                                                               |             |
| licenseProcessingState        | [licenseProcessingState](../resources/licenseprocessingstate.md)                      |             |
| mail                          | String                                                                                |             |
| mailEnabled                   | Boolean                                                                               |             |
| mailNickname                  | String                                                                                |             |
| mdmAppId                      | String                                                                                |             |
| membershipRule                | String                                                                                |             |
| membershipRuleProcessingState | String                                                                                |             |
| onPremisesDomainName          | String                                                                                |             |
| onPremisesLastSyncDateTime    | DateTimeOffset                                                                        |             |
| onPremisesNetBiosName         | String                                                                                |             |
| onPremisesProvisioningErrors  | [onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection |             |
| onPremisesSamAccountName      | String                                                                                |             |
| onPremisesSecurityIdentifier  | String                                                                                |             |
| onPremisesSyncEnabled         | Boolean                                                                               |             |
| preferredDataLocation         | String                                                                                |             |
| preferredLanguage             | String                                                                                |             |
| proxyAddresses                | String collection                                                                     |             |
| renewedDateTime               | DateTimeOffset                                                                        |             |
| resourceBehaviorOptions       | String collection                                                                     |             |
| resourceProvisioningOptions   | String collection                                                                     |             |
| securityEnabled               | Boolean                                                                               |             |
| securityIdentifier            | String                                                                                |             |
| theme                         | String                                                                                |             |
| visibility                    | String                                                                                |             |

## Response

If successful, this method returns a `200 OK` response code and a group object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_group"
}
-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}

Content-Type: application/json
Content-Length: 1987

{
  "@odata.type": "#microsoft.graph.group",
  "assignedLabels": [
    {
      "@odata.type": "#microsoft.graph.assignedLabel",
      "displayName": "String",
      "labelId": "String"
    }
  ],
  "assignedLicenses": [
    {
      "@odata.type": "#microsoft.graph.assignedLicense",
      "disabledPlans": [
        "Guid"
      ],
      "skuId": "Guid"
    }
  ],
  "classification": "String",
  "createdByAppId": "String",
  "createdDateTime": "DateTimeOffset",
  "deletedDateTime": "DateTimeOffset",
  "description": "String",
  "displayName": "String",
  "expirationDateTime": "DateTimeOffset",
  "groupTypes": [
    "String"
  ],
  "hasMembersWithLicenseErrors": "Boolean",
  "infoCatalogs": [
    "String"
  ],
  "isAssignableToRole": "Boolean",
  "licenseProcessingState": {
    "@odata.type": "#microsoft.graph.licenseProcessingState",
    "state": "String"
  },
  "mail": "String",
  "mailEnabled": "Boolean",
  "mailNickname": "String",
  "mdmAppId": "String",
  "membershipRule": "String",
  "membershipRuleProcessingState": "String",
  "onPremisesDomainName": "String",
  "onPremisesLastSyncDateTime": "DateTimeOffset",
  "onPremisesNetBiosName": "String",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "#microsoft.graph.onPremisesProvisioningError",
      "category": "String",
      "occurredDateTime": "DateTimeOffset",
      "propertyCausingError": "String",
      "value": "String"
    }
  ],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": "Boolean",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "proxyAddresses": [
    "String"
  ],
  "renewedDateTime": "DateTimeOffset",
  "resourceBehaviorOptions": [
    "String"
  ],
  "resourceProvisioningOptions": [
    "String"
  ],
  "securityEnabled": "Boolean",
  "securityIdentifier": "String",
  "theme": "String",
  "visibility": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.group"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.group",
  "assignedLabels": [
    {
      "@odata.type": "#microsoft.graph.assignedLabel",
      "displayName": "String",
      "labelId": "String"
    }
  ],
  "assignedLicenses": [
    {
      "@odata.type": "#microsoft.graph.assignedLicense",
      "disabledPlans": [
        "Guid"
      ],
      "skuId": "Guid"
    }
  ],
  "classification": "String",
  "createdByAppId": "String",
  "createdDateTime": "DateTimeOffset",
  "deletedDateTime": "DateTimeOffset",
  "description": "String",
  "displayName": "String",
  "expirationDateTime": "DateTimeOffset",
  "groupTypes": [
    "String"
  ],
  "hasMembersWithLicenseErrors": "Boolean",
  "id": "String(identifier)",
  "infoCatalogs": [
    "String"
  ],
  "isAssignableToRole": "Boolean",
  "licenseProcessingState": {
    "@odata.type": "#microsoft.graph.licenseProcessingState",
    "state": "String"
  },
  "mail": "String",
  "mailEnabled": "Boolean",
  "mailNickname": "String",
  "mdmAppId": "String",
  "membershipRule": "String",
  "membershipRuleProcessingState": "String",
  "onPremisesDomainName": "String",
  "onPremisesLastSyncDateTime": "DateTimeOffset",
  "onPremisesNetBiosName": "String",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "#microsoft.graph.onPremisesProvisioningError",
      "category": "String",
      "occurredDateTime": "DateTimeOffset",
      "propertyCausingError": "String",
      "value": "String"
    }
  ],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": "Boolean",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "proxyAddresses": [
    "String"
  ],
  "renewedDateTime": "DateTimeOffset",
  "resourceBehaviorOptions": [
    "String"
  ],
  "resourceProvisioningOptions": [
    "String"
  ],
  "securityEnabled": "Boolean",
  "securityIdentifier": "String",
  "theme": "String",
  "visibility": "String"
}
}

```