---
title: "recipient resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# recipient resource type

Namespace: microsoft.graph

## Properties

| Property     | Type                                         | Description |
| :----------- | :------------------------------------------- | :---------- |
| emailAddress | [emailAddress](../resources/emailaddress.md) |             |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.recipient",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.recipient",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}
```