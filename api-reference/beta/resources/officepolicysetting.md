# officepolicysetting resource type

Represents an Office policy setting.


### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|allowUserToModify|Boolean| **true** if the users are allowed to change configured settings; **false** if the settings are made mandatory. Supports $filter.    |
|category|String|The category of the setting. Read-only. Supports $filter.|
|comments|String|User defined comments. Supports $filter.|
|help|String|The help describes the details of the setting. Read-only. Supports $filter.|
|displayName|String|The displayName of the Office policy. This property is required when an Office policy is created and it cannot be cleared during updates. Read-only. Supports $filter and $orderby.|
|options|[policyOption](policyoption.md) collection|The options that are available for the policy setting. Read-only. Not nullable. |
|productName|String|The product name of the setting. Read-only. Supports $filter.|
|settingState|String|The officepolicysetting state: Draft = 0, Active = 1, Previous = 2. Possible values are: `Draft`, `Active`, `Previous`.|
|status|String|The officepolicysetting status: NotConfigured = 0, Enabled = 1, Disabled = 2. Possible values are: `NotConfigured`, `Enabled`, `Disabled`.|
|supportedOn|String|The supported Operating Systems. Read-only. Supports $filter.|

### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "allowUserToModify",
    "category",
    "comments",
    "displayName",
    "help",
    "settingState",
    "status",
    "supportedOn"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officepolicy"
}-->

```json
{
  "allowUserToModify": true,
  "category": "string",
  "comments": "string",
  "displayName": "string",
  "help": "string",
  "options": [{"@odata.type": "microsoft.graph.policyOption"}],
  "productName": "string",
  "settingState": "string",
  "status": "string",
  "supportedOn": "string"
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
