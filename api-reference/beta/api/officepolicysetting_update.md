# Update officePolicySetting

Update the properties of a officePolicySetting object. Only draft settings can be modified.

### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /officePolicies/<id>/settings/<id>
```
### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer <token>. Required. |

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|allowUserToModify|Boolean| **true** if the users are allowed to change configured settings; **false** if the settings are made mandatory. Supports $filter.    |
|comments|String|User defined comments. Supports $filter.|
|displayName|String|The displayName of the Office policy. This property is required when an Office policy is created and it cannot be cleared during updates. Supports $filter and $orderby.|
|options|[policyOption](policyoption.md) collection|The options that are available for the policy setting. Read-only. Not nullable. |
|status|String|The officepolicysetting status: NotConfigured = 0, Enabled = 1, Disabled = 2. Possible values are: `NotConfigured`, `Enabled`, `Disabled`.|

### Response
If successful, this method returns a `200 OK` response code and updated [officepolicysetting](../resources/officepolicysetting.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_officepolicy"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/officePolicies/<id>/settings/<id>
Content-type: application/json
Content-length: xxx

{
   "allowUserToModify": "allowUserToModify-value",
   "comments": "comments-value",
   "displayName": "displayName-value",
   "options": [
       "options-value"
   ],
   "status": "status-value"
}
```
##### Response
Here is an example of the response..
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
   "allowUserToModify": "allowUserToModify-value",
   "category": "category-value",
   "comments": "comments-value",
   "displayName": "displayName-value",
   "help": "help-value",
   "options": [
       "options-value"
   ],
   "status": "status-value",
   "supportedOn": "supportedOn-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
