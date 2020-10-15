---
title: "Create item"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Create item

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new outlookItem object.

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

In the request body, supply JSON representation of the [outlookItem](../resources/-outlookitem.md) object.

<!-- Actions and Functions -->

<!-- CRUD Methods -->

The following table shows the properties that are required when you create an outlookItem object.

| Property             | Type              | Description |
| :------------------- | :---------------- | :---------- |
| categories           | String collection |             |
| changeKey            | String            |             |
| createdDateTime      | DateTimeOffset    |             |
| id                   | String            | Read-only.  |
| lastModifiedDateTime | DateTimeOffset    |             |

## Response

If successful, this method returns a `201 Created` response code and an outlookItem object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "create_item"
}
-->

```http
POST https://graph.microsoft.com/beta

Content-Type: application/json
Content-Length: 2357

{
  "@odata.type": "#microsoft.graph.contact",
  "assistantName": "String",
  "birthday": "DateTimeOffset",
  "categories": [
    "String"
  ],
  "changeKey": "String",
  "children": [
    "String"
  ],
  "companyName": "String",
  "createdDateTime": "DateTimeOffset",
  "department": "String",
  "displayName": "String",
  "emailAddresses": [
    {
      "@odata.type": "#microsoft.graph.typedEmailAddress",
      "address": "String",
      "name": "String",
      "otherLabel": "String",
      "type": "String"
    }
  ],
  "fileAs": "String",
  "flag": {
    "@odata.type": "#microsoft.graph.followupFlag",
    "completedDateTime": {
      "@odata.type": "#microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    },
    "dueDateTime": {
      "@odata.type": "#microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    },
    "flagStatus": "String",
    "startDateTime": {
      "@odata.type": "#microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    }
  },
  "gender": "String",
  "generation": "String",
  "givenName": "String",
  "imAddresses": [
    "String"
  ],
  "initials": "String",
  "isFavorite": "Boolean",
  "jobTitle": "String",
  "lastModifiedDateTime": "DateTimeOffset",
  "manager": "String",
  "middleName": "String",
  "nickName": "String",
  "officeLocation": "String",
  "parentFolderId": "String",
  "personalNotes": "String",
  "phones": [
    {
      "@odata.type": "#microsoft.graph.phone",
      "number": "String",
      "type": "String"
    }
  ],
  "postalAddresses": [
    {
      "@odata.type": "#microsoft.graph.physicalAddress",
      "city": "String",
      "countryOrRegion": "String",
      "postOfficeBox": "String",
      "postalCode": "String",
      "state": "String",
      "street": "String",
      "type": "String"
    }
  ],
  "profession": "String",
  "spouseName": "String",
  "surname": "String",
  "title": "String",
  "websites": [
    {
      "@odata.type": "#microsoft.graph.website",
      "address": "String",
      "displayName": "String",
      "type": "String"
    }
  ],
  "weddingAnniversary": "Date",
  "yomiCompanyName": "String",
  "yomiGivenName": "String",
  "yomiSurname": "String"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.OutlookServices.outlookItem"
}
-->

```http
HTTP 1.1 201 Created

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.contact",
  "assistantName": "String",
  "birthday": "DateTimeOffset",
  "categories": [
    "String"
  ],
  "changeKey": "String",
  "children": [
    "String"
  ],
  "companyName": "String",
  "createdDateTime": "DateTimeOffset",
  "department": "String",
  "displayName": "String",
  "emailAddresses": [
    {
      "@odata.type": "#microsoft.graph.typedEmailAddress",
      "address": "String",
      "name": "String",
      "otherLabel": "String",
      "type": "String"
    }
  ],
  "fileAs": "String",
  "flag": {
    "@odata.type": "#microsoft.graph.followupFlag",
    "completedDateTime": {
      "@odata.type": "#microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    },
    "dueDateTime": {
      "@odata.type": "#microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    },
    "flagStatus": "String",
    "startDateTime": {
      "@odata.type": "#microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    }
  },
  "gender": "String",
  "generation": "String",
  "givenName": "String",
  "id": "String(identifier)",
  "imAddresses": [
    "String"
  ],
  "initials": "String",
  "isFavorite": "Boolean",
  "jobTitle": "String",
  "lastModifiedDateTime": "DateTimeOffset",
  "manager": "String",
  "middleName": "String",
  "nickName": "String",
  "officeLocation": "String",
  "parentFolderId": "String",
  "personalNotes": "String",
  "phones": [
    {
      "@odata.type": "#microsoft.graph.phone",
      "number": "String",
      "type": "String"
    }
  ],
  "postalAddresses": [
    {
      "@odata.type": "#microsoft.graph.physicalAddress",
      "city": "String",
      "countryOrRegion": "String",
      "postOfficeBox": "String",
      "postalCode": "String",
      "state": "String",
      "street": "String",
      "type": "String"
    }
  ],
  "profession": "String",
  "spouseName": "String",
  "surname": "String",
  "title": "String",
  "websites": [
    {
      "@odata.type": "#microsoft.graph.website",
      "address": "String",
      "displayName": "String",
      "type": "String"
    }
  ],
  "weddingAnniversary": "Date",
  "yomiCompanyName": "String",
  "yomiGivenName": "String",
  "yomiSurname": "String"
}
}

```