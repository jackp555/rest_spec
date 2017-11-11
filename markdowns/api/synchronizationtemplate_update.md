# Update synchronizationtemplate

Update the properties of synchronizationtemplate object.
## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) |    |
|Delegated (personal Microsoft account) |    |
|Application |  | 

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/<id>/synchronization/templates/<id>
PATCH /servicePrincipals/<id>/synchronization/templates/<id>
```
## Optional request headers
| Name       | Description|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|applicationId|Guid||
|default|Boolean||
|description|String||
|discoverable|Boolean||
|factoryTag|String||
|metadata|metadataEntry||

## Response
If successful, this method returns a `200 OK` response code and updated [synchronizationTemplate](../resources/synchronizationtemplate.md) object in the response body.
## Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_synchronizationtemplate"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/<id>/synchronization/templates/<id>
Content-type: application/json
Content-length: 161

{
  "applicationId": "applicationId-value",
  "default": true,
  "description": "description-value",
  "discoverable": true,
  "factoryTag": "factoryTag-value"
}
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 181

{
  "id": "id-value",
  "applicationId": "applicationId-value",
  "default": true,
  "description": "description-value",
  "discoverable": true,
  "factoryTag": "factoryTag-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationtemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->