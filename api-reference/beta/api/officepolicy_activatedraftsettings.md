# officePolicy: activateDraftSettings
Activates the settings that are currently set in the draftSettings property.  The active settings are then saved to the previousSettings property.

### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /officePolicies/<id>/activateDraftSettings
```
### Request headers
| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer <token>. Required.  |
| Content-Type  | application/json  |

### Request body
In the request body, provide a JSON object with the following parameters.

| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|
|securityEnabledOnly|Boolean|**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: The function can only be called on a user if the parameter is **true**.|

### Response
If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "user_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/officePolicies/<id>/activateDraftSettings
Content-type: application/json
Content-length: xxx

{
  "securityEnabledOnly": true
}
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "officePolicy: activateDraftSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
