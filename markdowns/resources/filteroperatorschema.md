# filterOperatorSchema resource type




## Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get filterOperatorSchema](../api/filteroperatorschema_get.md) | [filterOperatorSchema](filteroperatorschema.md) |Read properties and relationships of filterOperatorSchema object.|
|[Update](../api/filteroperatorschema_update.md) | [filterOperatorSchema](filteroperatorschema.md)	|Update filterOperatorSchema object. |
|[Delete](../api/filteroperatorschema_delete.md) | None |Delete filterOperatorSchema object. |

## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|arity|string| Possible values are: `Binary`, `Unary`.|
|multivaluedComparisonType|string| Possible values are: `All`, `Any`.|
|name|String| Read-only.|
|supportedAttributeTypes|string collection| Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

## Relationships
None


## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "string",
  "multivaluedComparisonType": "string",
  "name": "String (identifier)",
  "supportedAttributeTypes": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->