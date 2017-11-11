# synchronizationTemplate resource type




## Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get synchronizationTemplate](../api/synchronizationtemplate_get.md) | [synchronizationTemplate](synchronizationtemplate.md) |Read properties and relationships of synchronizationTemplate object.|
|[Update](../api/synchronizationtemplate_update.md) | [synchronizationTemplate](synchronizationtemplate.md)	|Update synchronizationTemplate object. |
|[Delete](../api/synchronizationtemplate_delete.md) | None |Delete synchronizationTemplate object. |

## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|applicationId|Guid||
|default|Boolean||
|description|String||
|discoverable|Boolean||
|factoryTag|String||
|id|String| Read-only.|
|metadata|[metadataEntry](metadataentry.md) collection||

## Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|schema|[synchronizationSchema](synchronizationschema.md)| Read-only. Nullable.|

## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}-->

```json
{
  "applicationId": "Guid",
  "default": true,
  "description": "String",
  "discoverable": true,
  "factoryTag": "String",
  "id": "String (identifier)",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->