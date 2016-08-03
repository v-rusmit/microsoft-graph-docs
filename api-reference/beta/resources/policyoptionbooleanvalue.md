# policyoptionbooleanvalue resource type

Represents an Office policy option boolean value. Inherits from [policyOption](policyoption.md).

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|defaultValue|boolean|The default value of the value.|
|label|string|The label of the option. Inherited from [policyOption](policyoption.md). Supports $filter.|
|value|boolean|The value to be set.|

### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "defaultValue",
    "label",
    "value",
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyoption"
}-->

```json
{
  "defaultValue": true,
  "label": "string",
  "value": true,
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
