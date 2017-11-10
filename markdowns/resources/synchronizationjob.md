# synchronizationJob resource type




## Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get synchronizationJob](../api/synchronizationjob_get.md) | [synchronizationJob](synchronizationjob.md) |Read properties and relationships of synchronizationJob object.|
|[Update](../api/synchronizationjob_update.md) | [synchronizationJob](synchronizationjob.md)	|Update synchronizationJob object. |
|[Delete](../api/synchronizationjob_delete.md) | None |Delete synchronizationJob object. |
|[Pause](../api/synchronizationjob_pause.md)|None||
|[Restart](../api/synchronizationjob_restart.md)|None||
|[Start](../api/synchronizationjob_start.md)|None||
|[Stop](../api/synchronizationjob_stop.md)|None||
|[Validatecredentials](../api/synchronizationjob_validatecredentials.md)|None||
|[Validatecredentials](../api/synchronizationjob_validatecredentials.md)|None||

## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|id|String| Read-only.|
|schedule|[synchronizationSchedule](synchronizationschedule.md)||
|status|[synchronizationStatus](synchronizationstatus.md)||
|templateId|String||

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
  "@odata.type": "microsoft.graph.synchronizationJob"
}-->

```json
{
  "id": "String (identifier)",
  "schedule": {"@odata.type": "microsoft.graph.synchronizationSchedule"},
  "status": {"@odata.type": "microsoft.graph.synchronizationStatus"},
  "templateId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->