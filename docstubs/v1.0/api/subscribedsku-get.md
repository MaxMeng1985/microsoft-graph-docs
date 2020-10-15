---
title: "Get subscribedSku"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Get subscribedSku

Namespace: microsoft.graph

Read the properties and relationships a subscribedSku object.

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

## Optional query parameters

This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Request Body

<!-- Actions and Functions -->

<!-- CRUD Methods -->

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a subscribedSku object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}
-->

```http
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.subscribedSku"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.subscribedSku",
  "appliesTo": "String",
  "capabilityStatus": "String",
  "consumedUnits": "Int32",
  "id": "String(identifier)",
  "prepaidUnits": {
    "@odata.type": "#microsoft.graph.licenseUnitsDetail",
    "enabled": "Int32",
    "suspended": "Int32",
    "warning": "Int32"
  },
  "servicePlans": [
    {
      "@odata.type": "#microsoft.graph.servicePlanInfo",
      "appliesTo": "String",
      "provisioningStatus": "String",
      "servicePlanId": "Guid",
      "servicePlanName": "String"
    }
  ],
  "skuId": "Guid",
  "skuPartNumber": "String"
}
}

```