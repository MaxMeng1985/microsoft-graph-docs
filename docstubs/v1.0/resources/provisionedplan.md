---
title: "provisionedPlan resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# provisionedPlan resource type

Namespace: microsoft.graph

## Properties

| Property           | Type   | Description |
| :----------------- | :----- | :---------- |
| capabilityStatus   | String |             |
| provisioningStatus | String |             |
| service            | String |             |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.provisionedPlan",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.provisionedPlan",
  "capabilityStatus": "String",
  "provisioningStatus": "String",
  "service": "String"
}
```