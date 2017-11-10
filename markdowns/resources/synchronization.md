# synchronization resource type




## Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get synchronization](../api/synchronization_get.md) | [synchronization](synchronization.md) |Read properties and relationships of synchronization object.|
|[Create synchronizationJob](../api/synchronization_post_jobs.md) |[synchronizationJob](synchronizationjob.md)| Create a new synchronizationJob by posting to the jobs collection.|
|[List jobs](../api/synchronization_list_jobs.md) |[synchronizationJob](synchronizationjob.md) collection| Get a synchronizationJob object collection.|
|[Create synchronizationTemplate](../api/synchronization_post_templates.md) |[synchronizationTemplate](synchronizationtemplate.md)| Create a new synchronizationTemplate by posting to the templates collection.|
|[List templates](../api/synchronization_list_templates.md) |[synchronizationTemplate](synchronizationtemplate.md) collection| Get a synchronizationTemplate object collection.|
|[Update](../api/synchronization_update.md) | [synchronization](synchronization.md)	|Update synchronization object. |
|[Delete](../api/synchronization_delete.md) | None |Delete synchronization object. |
|[Ping](../api/synchronization_ping.md)|String||

## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|secrets|[synchronizationSecretKeyStringValuePair](synchronizationsecretkeystringvaluepair.md) collection||
|version|String| Read-only.|

## Relationships
| Relationship | Type	|Description|
|:---------------|:--------|:----------|
|jobs|[synchronizationJob](synchronizationjob.md) collection| Read-only. Nullable.|
|templates|[synchronizationTemplate](synchronizationtemplate.md) collection| Read-only. Nullable.|

## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronization"
}-->

```json
{
  "secrets": [{"@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"}],
  "version": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->