# List jobs

Retrieve a list of synchronizationjob objects.
## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) |    |
|Delegated (personal Microsoft account) |    |
|Application |  | 

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /applications/<id>/synchronization/jobs
GET /servicePrincipals/<id>/synchronization/jobs
```
## Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.

## Request headers
| Name      |Description|
|:----------|:----------|
| Authorization  | Bearer {code}|

## Request body
Do not supply a request body for this method.
## Response
If successful, this method returns a `200 OK` response code and collection of [synchronizationJob](../resources/synchronizationjob.md) objects in the response body.
## Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_jobs"
}-->
```http
GET https://graph.microsoft.com/beta/applications/<id>/synchronization/jobs
```
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2958

{
  "value": [
    {
      "id": "id-value",
      "templateId": "templateId-value",
      "schedule": {
        "expiration": "datetime-value",
        "interval": "datetime-value",
        "state": "state-value"
      },
      "status": {
        "countSuccessiveCompleteFailures": 99,
        "escrowsPruned": true,
        "synchronizedEntryCountByType": [
          {
            "key": "key-value",
            "value": 99
          }
        ],
        "code": "code-value",
        "lastExecution": {
          "activityIdentifier": "activityIdentifier-value",
          "countEntitled": 99,
          "countEntitledForProvisioning": 99,
          "countEscrowed": 99,
          "countEscrowedRaw": 99,
          "countExported": 99,
          "countExports": 99,
          "countImported": 99,
          "countImportedDeltas": 99,
          "countImportedReferenceDeltas": 99,
          "state": "state-value",
          "error": {
            "code": "code-value",
            "message": "message-value",
            "tenantActionable": true
          },
          "timeBegan": "datetime-value",
          "timeEnded": "datetime-value"
        },
        "lastSuccessfulExecution": {
          "activityIdentifier": "activityIdentifier-value",
          "countEntitled": 99,
          "countEntitledForProvisioning": 99,
          "countEscrowed": 99,
          "countEscrowedRaw": 99,
          "countExported": 99,
          "countExports": 99,
          "countImported": 99,
          "countImportedDeltas": 99,
          "countImportedReferenceDeltas": 99,
          "state": "state-value",
          "error": {
            "code": "code-value",
            "message": "message-value",
            "tenantActionable": true
          },
          "timeBegan": "datetime-value",
          "timeEnded": "datetime-value"
        },
        "lastSuccessfulExecutionWithExports": {
          "activityIdentifier": "activityIdentifier-value",
          "countEntitled": 99,
          "countEntitledForProvisioning": 99,
          "countEscrowed": 99,
          "countEscrowedRaw": 99,
          "countExported": 99,
          "countExports": 99,
          "countImported": 99,
          "countImportedDeltas": 99,
          "countImportedReferenceDeltas": 99,
          "state": "state-value",
          "error": {
            "code": "code-value",
            "message": "message-value",
            "tenantActionable": true
          },
          "timeBegan": "datetime-value",
          "timeEnded": "datetime-value"
        },
        "steadyStateFirstAchievedTime": "datetime-value",
        "steadyStateLastAchievedTime": "datetime-value",
        "quarantine": {
          "currentBegan": "datetime-value",
          "nextAttempt": "datetime-value",
          "reason": "reason-value",
          "seriesBegan": "datetime-value",
          "seriesCount": 99
        },
        "troubleshootingUrl": "troubleshootingUrl-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->