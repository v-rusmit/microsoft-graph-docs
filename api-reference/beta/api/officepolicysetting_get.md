# Get officePolicySetting

Retrieve the properties and relationships of office policy setting object.

### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /officePolicies/<id>/<Product Name>/settings/<id>
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
GET https://graph.microsoft.com/v1.0/officePolicies/<id>/<Product Name>/settings/<id>
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
   "comment": "comment-value",
   "displayName": "displayName-value",
   "help": "description-value",
   "id": "id-value",
   "options": "description-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
