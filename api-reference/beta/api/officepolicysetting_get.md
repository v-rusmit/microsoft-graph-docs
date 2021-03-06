# Get officePolicySetting

Retrieve the properties and relationships of office policy setting object.

### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /officePolicies/<id>/settings/<id>
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
If successful, this method returns a `200 OK` response code and [officepolicysetting](../resources/officepolicysetting.md) object in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/beta/officePolicies/<id>/settings/<id>
```
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.officePolicySetting"
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
   "settingState": "settingState-value",
   "status": "status-value",
   "supportedOn": "supportedOn-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get officePolicySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
