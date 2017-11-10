# attributeMapping resource type




## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|defaultValue|String||
|exportMissingReferences|Boolean||
|flowBehavior|String| Possible values are: `FlowWhenChanged`, `FlowAlways`.|
|flowType|String| Possible values are: `Always`, `ObjectAddOnly`, `MultiValueAddOnly`.|
|matchingPriority|Int32||
|source|[attributeMappingSource](attributemappingsource.md)||
|targetAttributeName|String||

## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->