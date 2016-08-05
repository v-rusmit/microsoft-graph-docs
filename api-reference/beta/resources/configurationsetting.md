# configurationsetting resource type

Represents an Configuration Setting.


### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|category|String|The category of the setting. Read-only. Supports $filter.|
|help|String|The help describes the details of the setting. Read-only. Supports $filter.|
|displayName|String|The displayName of the Office policy. This property is required when an Office policy is created and it cannot be cleared during updates. Read-only. Supports $filter and $orderby.|
|options|[policyOption](policyoption.md) collection|The options that are available for the policy setting. Read-only. Not nullable. |
|productName|String|The product name of the setting. Read-only. Supports $filter.|
|supportedOn|String|The supported Operating Systems. Read-only. Supports $filter.|

### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "category",
    "displayName",
    "help",
    "productName",
    "supportedOn"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.configurationsetting"
}-->

```json
{
  "category": "string",
  "displayName": "string",
  "help": "string",
  "options": [{"@odata.type": "microsoft.graph.policyOption"}],
  "productName": "string",
  "supportedOn": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "configurationsetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
