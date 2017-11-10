# Create synchronizationTemplate

Use this API to create a new synchronizationTemplate.
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
POST /applications/<id>/synchronization/templates
POST /servicePrincipals/<id>/synchronization/templates

```
## Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer {code}|

## Request body
In the request body, supply a JSON representation of [synchronizationTemplate](../resources/synchronizationtemplate.md) object.


## Response
If successful, this method returns `201, Created` response code and [synchronizationTemplate](../resources/synchronizationtemplate.md) object in the response body.

## Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/<id>/synchronization/templates
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
In the request body, supply a JSON representation of [synchronizationTemplate](../resources/synchronizationtemplate.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->