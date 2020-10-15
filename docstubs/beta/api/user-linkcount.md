---
title: "user : linkCount"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# user : linkCount

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| Name          | Description               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Function Parameters

In the request url, provide the following query parameters with values.

<!-- Actions and Functions -->

The following table shows the parameters that can be used with this method.

| Parameter    | Type   | Description |
| :----------- | :----- | :---------- |
| relationship | String |             |

<!-- CRUD Methods -->

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 Ok` response code and a Int64 object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "user_linkcount"
}
-->

```http
GET https://graph.microsoft.com/beta/me/linkCount

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Int64"
}
-->

```http
HTTP 1.1 200 Ok

Content-Type: application/json
{
  "value": "Int64"
}

```