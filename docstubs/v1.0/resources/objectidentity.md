---
title: "objectIdentity resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# objectIdentity resource type

Namespace: microsoft.graph

## Properties

| Property         | Type   | Description |
| :--------------- | :----- | :---------- |
| issuer           | String |             |
| issuerAssignedId | String |             |
| signInType       | String |             |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.objectIdentity",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.objectIdentity",
  "issuer": "String",
  "issuerAssignedId": "String",
  "signInType": "String"
}
```