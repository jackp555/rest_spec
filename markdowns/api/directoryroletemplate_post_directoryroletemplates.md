# Create DirectoryRoleTemplate

Use this API to create a new DirectoryRoleTemplate.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoleTemplates

```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply a JSON representation of [DirectoryRoleTemplate](../resources/directoryroletemplate.md) object.


### Response
If successful, this method returns `201, Created` response code and [DirectoryRoleTemplate](../resources/directoryroletemplate.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_directoryroletemplate_from_directoryroletemplates"
}-->
```http
POST /directoryRoleTemplates
```
In the request body, supply a JSON representation of [DirectoryRoleTemplate](../resources/directoryroletemplate.md) object.
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryroletemplate"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 187

{
  "description": "description-value",
  "displayName": "displayName-value",
  "objectType": "objectType-value",
  "objectId": "objectId-value",
  "deletionTimestamp": "datetime-value"
}
```

<!-- uuid: ff604f14-3250-4c3c-b977-f8eb5bece1c4
2015-10-18 19:39:26 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create DirectoryRoleTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->