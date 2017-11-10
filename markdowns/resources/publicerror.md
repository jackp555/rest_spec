# publicError resource type




## Properties
| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|code|String||
|details|[publicErrorDetail](publicerrordetail.md) collection||
|innerError|[publicInnerError](publicinnererror.md)||
|message|String||
|target|String||

## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.publicError"
}-->

```json
{
  "code": "String",
  "details": [{"@odata.type": "microsoft.graph.publicErrorDetail"}],
  "innerError": {"@odata.type": "microsoft.graph.publicInnerError"},
  "message": "String",
  "target": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "publicError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->