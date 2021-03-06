# Get officePolicy

Retrieve the properties of the office policy object.

### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /officePolicies/<id>
```
### Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.
### Request headers
| Header       | Value|
|:-----------|:------|
| Authorization  | Bearer <token>. Required.|
| Accept  | application/json|

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and [officepolicy](../resources/officepolicy.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_officepolicy"
}-->
```http
GET https://graph.microsoft.com/beta/officePolicies/<id>
```
##### Response
Here is an example of the response. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
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
  "description": "Get officepolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
