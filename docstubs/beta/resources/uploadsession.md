---
title: "uploadSession resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# uploadSession resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Properties

| Property           | Type              | Description |
| :----------------- | :---------------- | :---------- |
| expirationDateTime | DateTimeOffset    |             |
| nextExpectedRanges | String collection |             |
| uploadUrl          | String            |             |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.uploadSession",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.uploadSession",
  "expirationDateTime": "DateTimeOffset",
  "nextExpectedRanges": ["String"],
  "uploadUrl": "String"
}
```