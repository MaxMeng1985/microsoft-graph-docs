---
title: "Create calendarPermissions"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create calendarPermissions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new calendarPermission object.

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

In the request body, supply JSON representation of the [calendarPermission](../resources/-calendarpermission.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a calendarPermission object.

| Property             | Type                                         | Description |
| :------------------- | :------------------------------------------- | :---------- |
| allowedRoles         | String collection                            |             |
| emailAddress         | [emailAddress](../resources/emailaddress.md) |             |
| id                   | String                                       | Read-only.  |
| isInsideOrganization | Boolean                                      |             |
| isRemovable          | Boolean                                      |             |
| role                 | String                                       |             |

## Response

If successful, this method returns a `201 Created` response code and a calendarPermission object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_calendarpermissions"
}
-->

```http
POST https://graph.microsoft.com/beta

Content-Type: application/json
Content-Length: 384

[
  {
    "@odata.type": "#microsoft.graph.calendarPermission",
    "allowedRoles": [
      "String"
    ],
    "emailAddress": {
      "@odata.type": "#microsoft.graph.emailAddress",
      "address": "String",
      "name": "String"
    },
    "id": "String(identifier)",
    "isInsideOrganization": "Boolean",
    "isRemovable": "Boolean",
    "role": "String"
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
    "@odata.type": "#microsoft.graph.calendarPermission",
    "allowedRoles": [
      "String"
    ],
    "emailAddress": {
      "@odata.type": "#microsoft.graph.emailAddress",
      "address": "String",
      "name": "String"
    },
    "id": "String(identifier)",
    "isInsideOrganization": "Boolean",
    "isRemovable": "Boolean",
    "role": "String"
  }
]
}

```