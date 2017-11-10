# Update filteroperatorschema

Update the properties of filteroperatorschema object.
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
PATCH /filterOperators/<name>
```
## Optional request headers
| Name       | Description|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|arity|string| Possible values are: `Binary`, `Unary`.|
|multivaluedComparisonType|string| Possible values are: `All`, `Any`.|
|supportedAttributeTypes|string| Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

## Response
If successful, this method returns a `200 OK` response code and updated [filterOperatorSchema](../resources/filteroperatorschema.md) object in the response body.
## Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_filteroperatorschema"
}-->
```http
PATCH https://graph.microsoft.com/beta/filterOperators/<name>
Content-type: application/json
Content-length: 166

{
  "arity": "arity-value",
  "multivaluedComparisonType": "multivaluedComparisonType-value",
  "supportedAttributeTypes": [
    "supportedAttributeTypes-value"
  ]
}
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.filterOperatorSchema"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 190

{
  "name": "name-value",
  "arity": "arity-value",
  "multivaluedComparisonType": "multivaluedComparisonType-value",
  "supportedAttributeTypes": [
    "supportedAttributeTypes-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update filteroperatorschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->