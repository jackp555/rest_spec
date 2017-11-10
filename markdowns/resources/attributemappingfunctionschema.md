# attributeMappingFunctionSchema resource type




## Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get attributeMappingFunctionSchema](../api/attributemappingfunctionschema_get.md) | [attributeMappingFunctionSchema](attributemappingfunctionschema.md) |Read properties and relationships of attributeMappingFunctionSchema object.|
|[Update](../api/attributemappingfunctionschema_update.md) | [attributeMappingFunctionSchema](attributemappingfunctionschema.md)	|Update attributeMappingFunctionSchema object. |
|[Delete](../api/attributemappingfunctionschema_delete.md) | None |Delete attributeMappingFunctionSchema object. |

## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|name|String| Read-only.|
|parameters|[attributeMappingParameterSchema](attributemappingparameterschema.md) collection||

## Relationships
None


## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}-->

```json
{
  "name": "String (identifier)",
  "parameters": [{"@odata.type": "microsoft.graph.attributeMappingParameterSchema"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->