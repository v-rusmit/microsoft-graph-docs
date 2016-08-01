# officepolicy resource type

Represents an Azure AD user account. Inherits from [directoryObject](directoryobject.md).


### Methods
| Method       | Return Type  |Description|
|:---------------|:--------|:----------|
|[Get officepolicy](../api/officepolicy_get.md) | [officepolicy](officepolicy.md) |Read properties of an officepolicy object.|
|[Update officepolicy](../api/officepolicy_update.md) | [officepolicy](officepolicy.md) |Update officepolicy object. |
|[Delete officepolicy](../api/officepolicy_delete.md) | None |Delete officepolicy object. |
|[List officepolicies](../api/officepolicy_list.md) |[officepolicy](officepolicy.md) collection| Get all the messages in the signed-in user's mailbox.|
|[Create officepolicy](../api/officepolicy_post_officepolcies.md) |[officepolicy](officepolicy.md)| Create a new Office Policy by posting to the office policies collection.|
|[Get officepolicysetting](../api/officepolicysetting_get.md) | [officepolicysetting](officepolicysetting.md) |Read properties of an officepolicysetting object.|
|[Update officepolicysetting](../api/officepolicysetting_update.md) | [officepolicysetting](officepolicysetting.md) |Update officepolicysetting object.|
|[Delete officepolicysetting](../api/officepolicysetting_delete.md) | None |Delete officepolicysetting object. |
|[List officepolicysettings](../api/officepolicy_list_officepolicysettings.md) |[officepolicysettings](officepolicysettings.md) collection| Get all the officepolicysettings in the officepolicy object.|

### Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|description|String|The user defined description of the Office policy. Supports $filter.|
|name|String|The name of the Office policy. This property is required when an Office policy is created and it cannot be cleared during updates. Supports $filter and $orderby.|


### JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignments",
    "calendar",
    "calendarGroups",
    "calendarView",
    "calendars",
    "contactFolders",
    "contacts",
    "createdObjects",
    "directReports",
    "drive",
    "events",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "messages",
    "oauth2PermissionGrants",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "registeredDevices"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}-->

```json
{
  "name": "string"
  "displayName": "string",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
