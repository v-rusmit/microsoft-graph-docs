# Create officePolicy

Use this API to create a new officePolicy as specified in the request body. 

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
|assignedGroups|[directoryObject](directoryobject.md) collection|The Office 365 Groups to which the policy is assigned. Supports $filter.|
|description|String|An optional description for the officePolicy. Supports $filter.|
|displayName|String|The name of the Office policy. This property is required when an Office policy is created and it cannot be cleared during updates. Supports $filter and $orderby.|
|policyEnabled|Boolean| **true** if the policy is enabled; otherwise, **false**. This property is required when a policy is created. Supports $filter.   |

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
POST https://graph.microsoft.com/beta/officePolicies
Content-type: application/json
Content-length: xxx

{
   "assignedGroups": [
      "assignedGroups-value"
    ],
   "description": "description-value",
   "displayName": "displayName-value",
   "policyEnabled": "policyEnabled-value"
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
  "description": "Create officepolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
