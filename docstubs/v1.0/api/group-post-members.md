---
title: "Add members"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Add members

Namespace: microsoft.graph

Add directoryObject by posting to the directoryObject collection.

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

In the request body, supply JSON representation of the [directoryObject](../resources/-directoryobject.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a directoryObject object.

| Property        | Type           | Description |
| :-------------- | :------------- | :---------- |
| deletedDateTime | DateTimeOffset |             |
| id              | String         | Read-only.  |

## Response

If successful, this method returns a `201 Created` response code and a directoryObject object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "add_members"
}
-->

```http
POST https://graph.microsoft.com/v1.0

Content-Type: application/json
Content-Length: 144

[
  {
    "@odata.type": "#microsoft.graph.directoryObject",
    "deletedDateTime": "DateTimeOffset",
    "id": "String(identifier)"
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
    "@odata.type": "#microsoft.graph.directoryObject",
    "deletedDateTime": "DateTimeOffset",
    "id": "String(identifier)"
  }
]
}

```