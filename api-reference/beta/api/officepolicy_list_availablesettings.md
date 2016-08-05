# List configurationSettings

List all the available configurationSettings available to be configured.

### HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /officepolicies/<Product Name>/configurationsettings
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
If successful, this method returns a `200 OK` response code and collection of [configurationSettings ](../resources/configurationsetting.md) objects in the response body.
### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_availableOfficePolicySettings"
}-->
```http
GET https://graph.microsoft.com/beta/officePolicies/<Product Name>/configurationsettings
```
##### Response
Here is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.configurationsetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

 {
  "value": [
   {
      "displayName": "displayName-value",
      "help": "help-value",
      "id": "id-value",
      "options": [
         "options-value"
      ],
      "supportedOn": "supportedOn-value"
   }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List configurationsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
