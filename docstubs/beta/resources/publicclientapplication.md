---
title: "publicClientApplication resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# publicClientApplication resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Properties

| Property     | Type              | Description |
| :----------- | :---------------- | :---------- |
| redirectUris | String collection |             |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicClientApplication",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.publicClientApplication",
  "redirectUris": ["String"]
}
```