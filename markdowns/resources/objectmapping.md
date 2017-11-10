# objectMapping resource type




## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|attributeMappings|[attributeMapping](attributemapping.md) collection||
|enabled|Boolean||
|flowTypes|String| Possible values are: `None`, `Add`, `Update`, `Delete`.|
|metadata|[metadataEntry](metadataentry.md) collection||
|name|String||
|scope|[filter](filter.md)||
|sourceObjectName|String||
|targetObjectName|String||

## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectMapping"
}-->

```json
{
  "attributeMappings": [{"@odata.type": "microsoft.graph.attributeMapping"}],
  "enabled": true,
  "flowTypes": "String",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "name": "String",
  "scope": {"@odata.type": "microsoft.graph.filter"},
  "sourceObjectName": "String",
  "targetObjectName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "objectMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->