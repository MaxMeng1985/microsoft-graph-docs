---
title: "Add claimsMappingPolicies"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Add claimsMappingPolicies

Namespace: microsoft.graph

Add claimsMappingPolicy by posting to the claimsMappingPolicy collection.

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

In the request body, supply JSON representation of the [claimsMappingPolicy](../resources/-claimsmappingpolicy.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a claimsMappingPolicy object.

| Property | Type | Description |
| :------- | :--- | :---------- |

## Response

If successful, this method returns a `201 Created` response code and a claimsMappingPolicy object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "add_claimsmappingpolicies"
}
-->

```http
POST https://graph.microsoft.com/v1.0

Content-Type: application/json
Content-Length: 294

[
  {
    "@odata.type": "#microsoft.graph.claimsMappingPolicy",
    "definition": [
      "String"
    ],
    "deletedDateTime": "DateTimeOffset",
    "description": "String",
    "displayName": "String",
    "id": "String(identifier)",
    "isOrganizationDefault": "Boolean"
  }
]

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "$(this.ReturnTypeFullName)"
}
-->

```http
HTTP 1.1 201 Created

Content-Type: application/json
{
  "value": [
  {
    "@odata.type": "#microsoft.graph.claimsMappingPolicy",
    "definition": [
      "String"
    ],
    "deletedDateTime": "DateTimeOffset",
    "description": "String",
    "displayName": "String",
    "id": "String(identifier)",
    "isOrganizationDefault": "Boolean"
  }
]
}

```