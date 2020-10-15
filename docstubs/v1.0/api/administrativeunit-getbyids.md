---
title: "administrativeunit : getByIds"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# administrativeunit : getByIds

Namespace: microsoft.graph

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

In the request body, supply JSON representation of the parameters.

<!-- Actions and Functions -->

The following table shows the parameters that can be used with this method.

| Parameter | Type              | Description |
| :-------- | :---------------- | :---------- |
| ids       | String collection |             |
| types     | String collection |             |

<!-- CRUD Methods -->

## Response

If successful, this method returns a `200 Ok` response code.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "administrativeunit_getbyids"
}
-->

```http
POST https://graph.microsoft.com/v1.0

```

### Response

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "$(this.ReturnTypeFullName)"
}
-->

```http
HTTP 1.1 200 Ok

```