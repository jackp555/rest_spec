# synchronizationSchema: parseExpression


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
POST /applications/<id>/synchronization/jobs/<id>/schema/parseExpression
POST /servicePrincipals/<id>/synchronization/jobs/<id>/schema/parseExpression
POST /applications/<id>/synchronization/templates/<id>/schema/parseExpression

```
## Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer {code}|

## Request body
In the request body, provide a JSON object with the following parameters.

| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|
|expression|String||
|testInputObject|expressionInputObject||
|targetAttributeDefinition|attributeDefinition||

## Response
If successful, this method returns `200, OK` response code and [parseExpressionResponse](../resources/parseexpressionresponse.md) object in the response body.

## Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "synchronizationschema_parseexpression"
}-->
```http
POST https://graph.microsoft.com/beta/applications/<id>/synchronization/jobs/<id>/schema/parseExpression
Content-type: application/json
Content-length: 1490

{
  "expression": "expression-value",
  "testInputObject": {
    "definition": {
      "attributes": [
        {
          "anchor": true,
          "caseExact": true,
          "defaultValue": "defaultValue-value",
          "metadata": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ],
          "multivalued": true,
          "mutability": "mutability-value",
          "name": "name-value",
          "required": true,
          "referencedObjects": [
            {
              "referencedObjectName": "referencedObjectName-value",
              "referencedProperty": "referencedProperty-value"
            }
          ],
          "type": "type-value"
        }
      ],
      "metadata": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ],
      "name": "name-value"
    },
    "properties": [
      {
        "key": "key-value"
      }
    ]
  },
  "targetAttributeDefinition": {
    "anchor": true,
    "caseExact": true,
    "defaultValue": "defaultValue-value",
    "metadata": [
      {
        "key": "key-value",
        "value": "value-value"
      }
    ],
    "multivalued": true,
    "mutability": "mutability-value",
    "name": "name-value",
    "required": true,
    "referencedObjects": [
      {
        "referencedObjectName": "referencedObjectName-value",
        "referencedProperty": "referencedProperty-value"
      }
    ],
    "type": "type-value"
  }
}
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.parseExpressionResponse"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 854

{
  "error": {
    "code": "code-value",
    "message": "message-value",
    "target": "target-value",
    "details": [
      {
        "code": "code-value",
        "message": "message-value",
        "target": "target-value"
      }
    ],
    "innerError": {
      "code": "code-value",
      "details": [
        {
          "code": "code-value",
          "message": "message-value",
          "target": "target-value"
        }
      ],
      "message": "message-value",
      "target": "target-value"
    }
  },
  "evaluationSucceeded": true,
  "evaluationResult": [
    "evaluationResult-value"
  ],
  "parsedExpression": {
    "expression": "expression-value",
    "name": "name-value",
    "parameters": [
      {
        "key": "key-value",
        "value": {
        }
      }
    ],
    "type": "type-value"
  },
  "parsingSucceeded": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema: parseExpression",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->