# officepolicy resource type

Represents an Office policy.


### Methods
| Method       | Return Type  |Description|
|:---------------|:--------|:----------|
|[Get officepolicy](../api/officepolicy_get.md) | [officepolicy](officepolicy.md) |Read properties of an officePolicy object.|
|[Update officepolicy](../api/officepolicy_update.md) | [officepolicy](officepolicy.md) |Update officePolicy object. |
|[Delete officepolicy](../api/officepolicy_delete.md) | None |Delete officepolicy object. |
|[List officepolicies](../api/officepolicy_list.md) |[officepolicy](officepolicy.md) collection| Get all the officepolicies in the organization.|
|[Create officepolicy](../api/officepolicy_post_officepolicies.md) |[officepolicy](officepolicy.md)| Create a new officePolicy by posting to the officePolicies collection.|
|[List availableofficepolicyproducts](../api/officepolicy_list_availableproducts.md) |[availableofficepolicyproduct](officepolicy_list_availablesettings.md) collection| List the available officePolicy products.|
|[List availableofficepolicysettings](../api/officepolicy_list_availablesettings.md) |[availableofficepolicysetting](availableofficepolicysetting.md) collection| List the available officePolicy settings.|
|[Get officepolicysetting](../api/officepolicysetting_get.md) | [officepolicysetting](officepolicysetting.md) |Read properties of an officePolicySetting object.|
|[Update officepolicysetting](../api/officepolicysetting_update.md) | [officepolicysetting](officepolicysetting.md) |Update officePolicySetting object.|
|[Delete officepolicysetting](../api/officepolicysetting_delete.md) | None |Delete officePolicySetting object. |
|[List officepolicysettings](../api/officepolicy_list_officepolicysettings.md) |[officepolicysetting](officepolicysettings.md) collection| Get all the officePolicySettings in the officePolicy object.|

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|description|String|An optional description for the officePolicy. Supports $filter.|
|name|String|The name of the Office policy. This property is required when an Office policy is created and it cannot be cleared during updates. Supports $filter and $orderby.|


### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "description",
    "displayName"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officepolicy"
}-->

```json
{
  "assignedGroups": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "description": "string",
  "displayName": "string"
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
