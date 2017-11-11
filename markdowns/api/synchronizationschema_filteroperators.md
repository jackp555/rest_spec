# synchronizationSchema: filterOperators


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
POST /applications/<id>/synchronization/jobs/<id>/schema/filterOperators
POST /servicePrincipals/<id>/synchronization/jobs/<id>/schema/filterOperators
POST /applications/<id>/synchronization/templates/<id>/schema/filterOperators

```
## Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer {code}|

## Request body

## Response
If successful, this method returns `200, OK` response code and [filterOperatorSchema](../resources/filteroperatorschema.md) collection object in the response body.

## Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_filteroperators"
}-->
```http
POST https://graph.microsoft.com/beta/applications/<id>/synchronization/jobs/<id>/schema/filterOperators
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.filterOperatorSchema",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 243

{
  "value": [
    {
      "name": "name-value",
      "arity": "arity-value",
      "multivaluedComparisonType": "multivaluedComparisonType-value",
      "supportedAttributeTypes": [
        "supportedAttributeTypes-value"
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: filterOperators",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->