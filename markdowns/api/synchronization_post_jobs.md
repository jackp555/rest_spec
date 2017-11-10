# Create synchronizationJob

Use this API to create a new synchronizationJob.
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
POST /applications/<id>/synchronization/jobs
POST /servicePrincipals/<id>/synchronization/jobs

```
## Request headers
| Name       | Description|
|:---------------|:----------|
| Authorization  | Bearer {code}|

## Request body
In the request body, supply a JSON representation of [synchronizationJob](../resources/synchronizationjob.md) object.


## Response
If successful, this method returns `201, Created` response code and [synchronizationJob](../resources/synchronizationjob.md) object in the response body.

## Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_synchronizationjob_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/<id>/synchronization/jobs
Content-type: application/json
Content-length: 2557

{
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
```
In the request body, supply a JSON representation of [synchronizationJob](../resources/synchronizationjob.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 2577

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create synchronizationJob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->