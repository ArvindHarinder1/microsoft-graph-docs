---
title: "statusDetails resource type"
description: "Describes the status of the provisioning event and the associated errors when status is set to failure."
localization_priority: Normal
author: "davidmu1"
ms.prod: "ms.prod"
doc_type: "resourcePageType"
---

# statusDetails resource type

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Describes the status of the provisioning event and the associated errors when status is set to failure. The status is inherited from [statusBase](../resources/statusBase.md). 

## Properties

| Property     | Type        | Description |
|:-------------|:------------|:------------|
|additionalDetails|String|Additional details in case of error.|
|errorCategory|String|Categorizes the error code.|
|errorCode|String|Unique error code if any occurred.|
|reason|String|Summarizes the status and describes why the status happened.|
|recommendedAction|String|Provides the resolution for the corresponding error.|
|status|String|Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.|

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusDetails",
  "baseType": "self.statusBase"
}-->

```json
{
  "additionalDetails": "String",
  "errorCategory": "String",
  "errorCode": "String",
  "reason": "String",
  "recommendedAction": "String",
   "status": "failure"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
