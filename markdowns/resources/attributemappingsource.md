# attributeMappingSource resource type




## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|expression|String||
|name|String||
|parameters|[stringKeyAttributeMappingSourceValuePair](stringkeyattributemappingsourcevaluepair.md) collection||
|type|String| Possible values are: `Attribute`, `Constant`, `Function`.|

## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
  "expression": "String",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"}],
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->