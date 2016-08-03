# policyoptionvalue resource type

Represents an Office policy option value. Inherits from [policyOption](policyoption.md).


### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|defaultValue|String|The default value of the value. Inherited from [policyOption](policyoption.md).|
|label|String|The label of the option. Inherited from [policyOption](policyoption.md). Supports $filter.|
|valueType|string|The value type: String = 0, Boolean = 1, Integer = 2, . Possible values are: `String`, `Boolean`, `Integer`.|
|value|String|The value to be set. Inherited from [policyOption](policyoption.md). Supports $filter.|

### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "defaultValue",
    "label",
    "valueType",
    "value"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyoption"
}-->

```json
{
  "defaultValue": "string",
  "label": "string",
  "valueType": "string",
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
