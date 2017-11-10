# Update synchronizationjob

Update the properties of synchronizationjob object.
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
PATCH /applications/<id>/synchronization/jobs/<id>
PATCH /servicePrincipals/<id>/synchronization/jobs/<id>
```
## Optional request headers
| Name       | Description|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## Request body
In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.

| Property	   | Type	|Description|
|:---------------|:--------|:----------|
|schedule|synchronizationSchedule||
|status|synchronizationStatus||
|templateId|String||

## Response
If successful, this method returns a `200 OK` response code and updated [synchronizationJob](../resources/synchronizationjob.md) object in the response body.
## Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_synchronizationjob"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/<id>/synchronization/jobs/<id>
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
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationJob"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "Update synchronizationjob",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->