# Create officePolicySetting

Use this API to create a new officePolicySetting as specified in the request body.

### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /officePolicies
```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer <token>. Required. |

### Request body
In the request body, supply a JSON representation of [configurationSetting](../resources/configurationsetting.md) object.

### Response
If successful, this method returns `201, Created` response code and [officePolicySetting](../resources/officepolicysetting.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_officepolicysetting_from_configurationsetting"
}-->
```http
POST https://graph.microsoft.com/beta/officepolicies/<id>/settings
Content-type: application/json
Content-length: xxx

{
  "configurationSetting": {
  }
}
```
In the request body, supply a JSON representation of [directoryObject](../resources/configurationsetting.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.officepolicysetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
   "assignedGroups": [
      "assignedGroups-value"
    ],
   "displayName": "displayName-value",
   "description": "description-value",
   "id": "id-value",
   "policyEnabled": "policyEnabled-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create officepolicysetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
