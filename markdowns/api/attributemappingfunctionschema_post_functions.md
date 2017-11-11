# Create attributeMappingFunctionSchema

Use this API to create a new attributeMappingFunctionSchema.
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
POST /functions

```
## Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer {code}|

## Request body
In the request body, supply a JSON representation of [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.


## Response
If successful, this method returns `201, Created` response code and [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object in the response body.

## Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_attributemappingfunctionschema_from_functions"
}-->
```http
POST https://graph.microsoft.com/beta/functions
Content-type: application/json
Content-length: 156

{
  "parameters": [
    {
      "allowMultipleOccurrences": true,
      "name": "name-value",
      "required": true,
      "type": "type-value"
    }
  ]
}
```
In the request body, supply a JSON representation of [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 180

{
  "name": "name-value",
  "parameters": [
    {
      "allowMultipleOccurrences": true,
      "name": "name-value",
      "required": true,
      "type": "type-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create attributeMappingFunctionSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->