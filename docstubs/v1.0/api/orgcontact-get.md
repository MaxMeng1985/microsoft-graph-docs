---
title: "Get orgContact"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Get orgContact

Namespace: microsoft.graph

Read the properties and relationships an orgContact object.

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

If successful, this method returns a `200 OK` response code and an orgContact object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}
-->

```http
GET https://graph.microsoft.com/v1.0/contacts/{id}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.orgContact"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.orgContact",
  "addresses": [
    {
      "@odata.type": "#microsoft.graph.physicalOfficeAddress",
      "city": "String",
      "countryOrRegion": "String",
      "officeLocation": "String",
      "postalCode": "String",
      "state": "String",
      "street": "String"
    }
  ],
  "companyName": "String",
  "deletedDateTime": "DateTimeOffset",
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "id": "String(identifier)",
  "jobTitle": "String",
  "mail": "String",
  "mailNickname": "String",
  "onPremisesLastSyncDateTime": "DateTimeOffset",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "#microsoft.graph.onPremisesProvisioningError",
      "category": "String",
      "occurredDateTime": "DateTimeOffset",
      "propertyCausingError": "String",
      "value": "String"
    }
  ],
  "onPremisesSyncEnabled": "Boolean",
  "phones": [
    {
      "@odata.type": "#microsoft.graph.phone",
      "language": "String",
      "number": "String",
      "region": "String",
      "type": "String"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "surname": "String"
}
}

```