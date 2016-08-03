# Update officePolicy

Update the properties of a officePolicy object.
### Prerequisites
The following **scope** is required to execute this API: *OfficePolicy.ReadWrite.All*

### HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /officePolicies/<id>
```
### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer <token>. Required. |

### Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|description|String|An optional description for the group. |
|displayName|String|The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.|

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
PATCH https://graph.microsoft.com/v1.0/officePolicies/<id>
Content-type: application/json
Content-length: xxx

{
   "assignedGroups": [
      "assignedGroups-value"
    ],
   "description": "description-value",
   "displayName": "displayName-value",
   "id": "id-value"
}
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
   "id": "id-value"
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