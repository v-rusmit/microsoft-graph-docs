# List officePolicySettings

List all the officePolicySetting available in an organization.

### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /officePolicies/<id>/settings/active
GET /officePolicies/<id>/settings/draft
GET /officePolicies/<id>/settings/previous
```
### Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.
### Request headers
| Name       | Type | Description|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer <token>. Required. |

### Request body
Do not supply a request body for this method.
### Response
If successful, this method returns a `200 OK` response code and collection of [officepolicysetting](../resources/officepolicysetting.md) objects in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_officepolicies"
}-->
```http
GET https://graph.microsoft.com/beta/officePolicies/<id>/settings/active
```
##### Response
Here is an example of the response.

Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.officepolicysetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
    {
      "allowUserToModify": "allowUserToModify-value",
      "category": "category-value",
      "comments": "comments-value",
      "displayName": "displayName-value",
      "help": "help-value",
      "id": "id-value",
      "options": [
       "options-value"
      ],
      "status": "status-value",
      "supportedOn": "supportedOn-value"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List officepolicysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
