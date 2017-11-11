# synchronizationSchema resource type




## Methods

| Method		   | Return Type	|Description|
|:---------------|:--------|:----------|
|[Get synchronizationSchema](../api/synchronizationschema_get.md) | [synchronizationSchema](synchronizationschema.md) |Read properties and relationships of synchronizationSchema object.|
|[Update](../api/synchronizationschema_update.md) | [synchronizationSchema](synchronizationschema.md)	|Update synchronizationSchema object. |
|[Delete](../api/synchronizationschema_delete.md) | None |Delete synchronizationSchema object. |
|[Filteroperators](../api/synchronizationschema_filteroperators.md)|[filterOperatorSchema](filteroperatorschema.md) collection||
|[Functions](../api/synchronizationschema_functions.md)|[attributeMappingFunctionSchema](attributemappingfunctionschema.md) collection||
|[Parseexpression](../api/synchronizationschema_parseexpression.md)|[parseExpressionResponse](parseexpressionresponse.md)||

## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|directories|[directoryDefinition](directorydefinition.md) collection||
|provisioningTaskIdentifier|String| Read-only.|
|synchronizationRules|[synchronizationRule](synchronizationrule.md) collection||
|version|String||

## Relationships
None


## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSchema"
}-->

```json
{
  "directories": [{"@odata.type": "microsoft.graph.directoryDefinition"}],
  "provisioningTaskIdentifier": "String (identifier)",
  "synchronizationRules": [{"@odata.type": "microsoft.graph.synchronizationRule"}],
  "version": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->