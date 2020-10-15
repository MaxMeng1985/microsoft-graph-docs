---
title: "Create outlookCategory"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create outlookCategory

Namespace: microsoft.graph

Create a new outlookCategory object.

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

In the request body, supply JSON representation of the [outlookCategory](../resources/-outlookcategory.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create an outlookCategory object.

| Property    | Type   | Description |
| :---------- | :----- | :---------- |
| color       | String |             |
| displayName | String |             |
| id          | String | Read-only.  |

## Response

If successful, this method returns a `201 Created` response code and an outlookCategory object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_outlookcategory"
}
-->

```http
POST https://graph.microsoft.com/v1.0/users/{id}/outlook/masterCategories/{id}

Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.outlookCategory",
  "color": "String",
  "displayName": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.OutlookServices.outlookCategory"
}
-->

```http
HTTP 1.1 201 Created

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.outlookCategory",
  "color": "String",
  "displayName": "String",
  "id": "String(identifier)"
}
}

```