---
title: "Update calendars"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update calendars

Namespace: microsoft.graph

Update the properties of a calendar object.

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

In the request body, supply JSON representation of the [calendar](../resources/-calendar.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a calendar object.

| Property                      | Type                                         | Description |
| :---------------------------- | :------------------------------------------- | :---------- |
| allowedOnlineMeetingProviders | String collection                            |             |
| canEdit                       | Boolean                                      |             |
| canShare                      | Boolean                                      |             |
| canViewPrivateItems           | Boolean                                      |             |
| changeKey                     | String                                       |             |
| color                         | String                                       |             |
| defaultOnlineMeetingProvider  | String                                       |             |
| hexColor                      | String                                       |             |
| id                            | String                                       | Read-only.  |
| isDefaultCalendar             | Boolean                                      |             |
| isRemovable                   | Boolean                                      |             |
| isTallyingResponses           | Boolean                                      |             |
| name                          | String                                       |             |
| owner                         | [emailAddress](../resources/emailaddress.md) |             |

## Response

If successful, this method returns a `200 OK` response code and a calendar object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_calendars"
}
-->

```http
PATCH https://graph.microsoft.com/v1.0

Content-Type: application/json
Content-Length: 640

[
  {
    "@odata.type": "#microsoft.graph.calendar",
    "allowedOnlineMeetingProviders": [
      "String"
    ],
    "canEdit": "Boolean",
    "canShare": "Boolean",
    "canViewPrivateItems": "Boolean",
    "changeKey": "String",
    "color": "String",
    "defaultOnlineMeetingProvider": "String",
    "hexColor": "String",
    "id": "String(identifier)",
    "isDefaultCalendar": "Boolean",
    "isRemovable": "Boolean",
    "isTallyingResponses": "Boolean",
    "name": "String",
    "owner": {
      "@odata.type": "#microsoft.graph.emailAddress",
      "address": "String",
      "name": "String"
    }
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
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": [
  {
    "@odata.type": "#microsoft.graph.calendar",
    "allowedOnlineMeetingProviders": [
      "String"
    ],
    "canEdit": "Boolean",
    "canShare": "Boolean",
    "canViewPrivateItems": "Boolean",
    "changeKey": "String",
    "color": "String",
    "defaultOnlineMeetingProvider": "String",
    "hexColor": "String",
    "id": "String(identifier)",
    "isDefaultCalendar": "Boolean",
    "isRemovable": "Boolean",
    "isTallyingResponses": "Boolean",
    "name": "String",
    "owner": {
      "@odata.type": "#microsoft.graph.emailAddress",
      "address": "String",
      "name": "String"
    }
  }
]
}

```