# Update officePolicy

Update the properties of a officePolicy object.

### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /officePolicies/<id>
```
### Request headers
| Header       | Value|
|:-----------|:------|
| Authorization  | Bearer <token>. Required.  |
| Content-Type  | application/json  |

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|
|assignedGroups|[directoryObject](directoryobject.md) collection|The Office 365 Groups to which the policy is assigned. Supports $filter.|
|description|String|An optional description for the officePolicy. Supports $filter.|
|displayName|String|The name of the Office policy. This property is required when an Office policy is created and it cannot be cleared during updates. Supports $filter and $orderby.|
|policyEnabled|Boolean| **true** if the policy is enabled; otherwise, **false**. This property is required when a policy is created. Supports $filter.   |
|settings|[officePolicySetting](officepolicysetting.md) collection|The Office Policy settings that have been modified but not been applied to the policy. Supports $filter.|

### Response
If successful, this method returns a `200 OK` response code and updated [officepolicy](../resources/officepolicy.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_officepolicy"
}-->
```http
PATCH https://graph.microsoft.com/beta/officePolicies/<id>
Content-type: application/json
Content-length: xxx

{
   "assignedGroups": [
      "assignedGroups-value"
    ],
   "category": "category-value",
   "description": "description-value",
   "displayName": "displayName-value",
   "policyEnabled": "policyEnabled-value",
   "settings": [
      "draftSettings-value"
    ],
}
```
##### Response
Here is an example of the response. 
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
   "assignedGroups": [
      "assignedGroups-value"
    ],
   "description": "description-value",
   "displayName": "displayName-value",
   "id": "id-value",
   "policyEnabled": "policyEnabled-value",
   "settings": [
      "settings-value"
    ],
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
