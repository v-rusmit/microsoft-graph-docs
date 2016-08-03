# policyoption resource type

Represents an Office policy option.


### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|allowUserToModify|Boolean| **true** if the users are allowed to change configured settings; **false** if the settings are made mandatory. Supports $filter.    |
|label|String|The label of the option. Supports $filter.|
|valueType|string|The value type: String = 0, Boolean = 1, Integer = 2, . Possible values are: `String`, `Boolean`, `Integer`.|
|value|String|The value to be set. Supports $filter.|

### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "allowUserToModify",
    "comments",
    "displayName",
    "help",
    "status",
    "supportedOn"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyoption"
}-->

```json
{
  "allowUserToModify": true,
  "comments": "string",
  "displayName": "string",
  "help": "string",
  "options": [{"@odata.type": "microsoft.graph.policyOption"}],
  "status": "string",
  "supportedOn": "string"
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
