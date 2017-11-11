# Get synchronizationSchema

Retrieve the properties and relationships of synchronizationschema object.
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
GET /applications/<id>/synchronization/jobs/<id>/schema
GET /servicePrincipals/<id>/synchronization/jobs/<id>/schema
GET /applications/<id>/synchronization/templates/<id>/schema
```
## Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.

## Request headers
| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer {code}|

## Request body
Do not supply a request body for this method.
## Response
If successful, this method returns a `200 OK` response code and [synchronizationSchema](../resources/synchronizationschema.md) object in the response body.
## Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/applications/<id>/synchronization/jobs/<id>/schema
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 4154

{
  "provisioningTaskIdentifier": "provisioningTaskIdentifier-value",
  "directories": [
    {
      "id": "id-value",
      "name": "name-value",
      "objects": [
        {
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
        }
      ]
    }
  ],
  "synchronizationRules": [
    {
      "editable": true,
      "id": "id-value",
      "metadata": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ],
      "name": "name-value",
      "objectMappings": [
        {
          "attributeMappings": [
            {
              "defaultValue": "defaultValue-value",
              "exportMissingReferences": true,
              "flowBehavior": "flowBehavior-value",
              "flowType": "flowType-value",
              "matchingPriority": 99,
              "source": {
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
              "targetAttributeName": "targetAttributeName-value"
            }
          ],
          "enabled": true,
          "flowTypes": "flowTypes-value",
          "metadata": [
            {
              "key": "key-value",
              "value": "value-value"
            }
          ],
          "name": "name-value",
          "scope": {
            "groups": [
              {
                "clauses": [
                  {
                    "operatorName": "operatorName-value",
                    "sourceOperandName": "sourceOperandName-value",
                    "targetOperand": {
                      "values": [
                        "values-value"
                      ]
                    }
                  }
                ],
                "name": "name-value"
              }
            ],
            "inputFilterGroups": [
              {
                "clauses": [
                  {
                    "operatorName": "operatorName-value",
                    "sourceOperandName": "sourceOperandName-value",
                    "targetOperand": {
                      "values": [
                        "values-value"
                      ]
                    }
                  }
                ],
                "name": "name-value"
              }
            ],
            "categoryFilterGroups": [
              {
                "clauses": [
                  {
                    "operatorName": "operatorName-value",
                    "sourceOperandName": "sourceOperandName-value",
                    "targetOperand": {
                      "values": [
                        "values-value"
                      ]
                    }
                  }
                ],
                "name": "name-value"
              }
            ]
          },
          "sourceObjectName": "sourceObjectName-value",
          "targetObjectName": "targetObjectName-value"
        }
      ],
      "priority": 99,
      "sourceDirectoryName": "sourceDirectoryName-value",
      "targetDirectoryName": "targetDirectoryName-value"
    }
  ],
  "version": "version-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get synchronizationSchema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->