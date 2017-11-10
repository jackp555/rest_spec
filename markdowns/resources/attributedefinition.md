# attributeDefinition resource type




## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|anchor|Boolean||
|caseExact|Boolean||
|defaultValue|String||
|metadata|[metadataEntry](metadataentry.md) collection||
|multivalued|Boolean||
|mutability|String| Possible values are: `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.|
|name|String||
|referencedObjects|[referencedObject](referencedobject.md) collection||
|required|Boolean||
|type|String| Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|

## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeDefinition"
}-->

```json
{
  "anchor": true,
  "caseExact": true,
  "defaultValue": "String",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "multivalued": true,
  "mutability": "String",
  "name": "String",
  "referencedObjects": [{"@odata.type": "microsoft.graph.referencedObject"}],
  "required": true,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->