# officepolicysetting resource type

Represents an Office policy setting.


### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|allowUserToModify|Boolean| **true** if the users are allowed to change configured settings; **false** if the settings are made mandatory. Supports $filter.    |
|description|String|An optional description for the officePolicy. Supports $filter.|
|name|String|The name of the Office policy. This property is required when an Office policy is created and it cannot be cleared during updates. Supports $filter and $orderby.|
|status|string|The officepolicysetting status: NotConfigured = 0, Enabled = 1, Disabled = 2. Possible values are: `NotConfigured`, `Enabled`, `Disabled`.|


### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "allowUserToModify",
    "description",
    "displayName",
    "status"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officepolicy"
}-->

```json
{
  "allowUserToModify": true,
  "description": "string",
  "displayName": "string",
  "status": "string"
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
