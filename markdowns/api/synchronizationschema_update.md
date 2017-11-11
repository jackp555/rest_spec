# Update synchronizationschema

Update the properties of synchronizationschema object.
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
PATCH /applications/<id>/synchronization/jobs/<id>/schema
PATCH /servicePrincipals/<id>/synchronization/jobs/<id>/schema
PATCH /applications/<id>/synchronization/templates/<id>/schema
```
## Optional request headers
| Name       | Description|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|directories|directoryDefinition||
|synchronizationRules|synchronizationRule||
|version|String||

## Response
If successful, this method returns a `200 OK` response code and updated [synchronizationSchema](../resources/synchronizationschema.md) object in the response body.
## Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_synchronizationschema"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/<id>/synchronization/jobs/<id>/schema
Content-type: application/json
Content-length: 4086

{
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
  "description": "Update synchronizationschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->