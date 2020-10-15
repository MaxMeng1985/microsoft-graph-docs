---
title: "Update conversation"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update conversation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a conversation object.

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

In the request body, supply JSON representation of the [conversation](../resources/-conversation.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create a conversation object.

| Property              | Type              | Description |
| :-------------------- | :---------------- | :---------- |
| hasAttachments        | Boolean           |             |
| id                    | String            | Read-only.  |
| lastDeliveredDateTime | DateTimeOffset    |             |
| preview               | String            |             |
| topic                 | String            |             |
| uniqueSenders         | String collection |             |

## Response

If successful, this method returns a `200 OK` response code and a conversation object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_conversation"
}
-->

```http
PATCH https://graph.microsoft.com/beta/groups/{id}/conversations/{id}

Content-Type: application/json
Content-Length: 220

{
  "@odata.type": "#microsoft.graph.conversation",
  "hasAttachments": "Boolean",
  "lastDeliveredDateTime": "DateTimeOffset",
  "preview": "String",
  "topic": "String",
  "uniqueSenders": [
    "String"
  ]
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.OutlookServices.conversation"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.conversation",
  "hasAttachments": "Boolean",
  "id": "String(identifier)",
  "lastDeliveredDateTime": "DateTimeOffset",
  "preview": "String",
  "topic": "String",
  "uniqueSenders": [
    "String"
  ]
}
}

```