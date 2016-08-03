# officepolicyproduct resource type

Represents an Office policy product.

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|displayName|String|The display name of the Office policy product. This property is required when an Office policy is created and it cannot be cleared during updates. Supports $filter and $orderby.|

### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officepolicy"
}-->

```json
{
  "displayName": "string",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "officePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->