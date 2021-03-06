# policyoptionnumericvalue resource type

Represents an Office policy option numeric value. Inherits from [policyOption](policyoption.md).


### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|defaultValue|string|The default value of the value.|
|label|string|The label of the option. Inherited from [policyOption](policyoption.md). Supports $filter.|
|maximumValue|number|The maximum numeric value allowed. Supports $filter.|
|minimumValue|number|The minimum numeric value allowed. Supports $filter.|
|increment|number|The numeric increment between values. Supports $filter.|
|value|string|The value to be set. Supports $filter.|

### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "defaultValue",
    "increment",
    "label",
    "minimumValue",
    "maximumValue",
    "value"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyoption"
}-->

```json
{
  "defaultValue": "string",
  "increment": 1024,
  "label": "string",
  "minimumValue": 1024,
  "maximumValue": 1024,
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policyoption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
