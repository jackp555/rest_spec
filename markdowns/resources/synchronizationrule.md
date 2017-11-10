# synchronizationRule resource type




## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|editable|Boolean||
|id|String||
|metadata|[stringKeyStringValuePair](stringkeystringvaluepair.md) collection||
|name|String||
|objectMappings|[objectMapping](objectmapping.md) collection||
|priority|Int32||
|sourceDirectoryName|String||
|targetDirectoryName|String||

## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationRule"
}-->

```json
{
  "editable": true,
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objectMappings": [{"@odata.type": "microsoft.graph.objectMapping"}],
  "priority": 1024,
  "sourceDirectoryName": "String",
  "targetDirectoryName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->