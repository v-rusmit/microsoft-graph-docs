# Create officePolicy

Use this API to create a new officePolicy as specified in the request body. 

### Prerequisites
The following **scope** is required to execute this API: _OfficePolicy.ReadWrite.All_ 
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
In the request body, supply a JSON representation of [officePolicy](../resources/officepolicy.md) object.

The following table shows the properties that are required when you create a group.

| Parameter | Type | Description|
|:---------------|:--------|:----------|
| displayName | string | The name to display in the address book for the group. |
| mailEnabled | boolean | Set to **true** for mail-enabled groups. |
| mailNickname | string | The mail alias for the group. |
| securityEnabled | boolean | Set to **true** for security-enabled groups. Set to **false** if creating an Office 365 group. |

### Response
If successful, this method returns `201, Created` response code and [officePolicy](../resources/officepolicy.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_officePolicy_from_officePolicoes"
}-->
```http
POST https://graph.microsoft.com/v1.0/officePolicies
Content-type: application/json
Content-length: xxx

{
  "description": "description-value",
  "displayName": "displayName-value",
}
```
In the request body, supply a JSON representation of [officePolicy](../resources/officepolicy.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.officepolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "description": "description-value",
  "displayName": "displayName-value",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create officepolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
