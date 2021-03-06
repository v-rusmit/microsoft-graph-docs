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

### Request body
Do not supply a request body for this method.

### Response
If successful, this method returns `200, OK` response code and String collection in the response body that contains the IDs of the groups that the user is a member of.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "officepolicy_activatedraftsettings"
}-->
```http
POST https://graph.microsoft.com/beta/officePolicies/<id>/activateDraftSettings
```

##### Response

Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
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
